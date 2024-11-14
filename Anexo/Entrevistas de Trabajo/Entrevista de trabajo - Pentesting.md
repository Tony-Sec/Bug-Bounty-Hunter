
###### Después de meter mimikatz en el objetivo, dumpeamos la SAM ,¿estos hashes NTLM son del dominio o de la máquina local?
- Máquina local
###### En una auditoria web ,¿Cómo podemos probar un CSRF?
- Necesitamos de la interacción de una tercera persona.

	Estamos logeados en una web y capturamos la petición de cambio de contraseña (con Burp) que normalmente viaja por POST (en forma de data) y la cambiamos a GET para que el parámetro aparezca en la url. 

	Una vez tenemos la url de cambio de contraseña con GET ,accedemos a ella y nos cambia la contraseña, el siguiente paso sería enviarle la url a la víctima (con un acortador) y si está logeada en la web ,le habremos cambiado la contraseña de forma exitosa.

# Teniendo un objetivo vulnerable a LFI:
Si tengo un local file inclusion ,quiere decir que el servidor me 
permite leer archivos del sistema a través de una variable parametrizada en la url:
`http://<SERVER_IP>:<PORT>/index.php?language=es.php` -> `http://<SERVER_IP>:<PORT>/index.php?language=/etc/passwd`
## ¿Cómo se visualizaría un archivo PHP, es decir, ver el código del recurso ?

Si apuntamos por ejemplo al archivo php directamente en la url se nos va a interpretar por lo que es necesario utilizar:
### Wrappers
Utilizamos en la url un wrapper en base64 para codificar el script y así que se nos muestre codificado y después descodificarlo en local.
## ¿Cómo se podría ganar acceso al sistema desde un LFI?

### Reverse shell - muy básico
Puedo subir un archivo que contenga una reverse shell y así transformar la vulnerabilidad en un remote code execution.
### ID RSA por ssh - básico
Leemos /etc/passwd y vemos los usuarios del sistema, nos dirigimos al directorio .ssh (donde está el par de claves) y a lo mejor vemos un ID RSA de algún usuario válido con el que podemos ganar acceso de forma externa sin proporcionar contraseña.
### Log poisoning - avanzado
Leemos algún log del sistema (de Apache `/var/log/apache2/acess.log` o ssh `/var/log/auth.log`) y vemos el User Agent de las peticiones ,manipulamos (con Burp) el User Agent de las peticiones  que realizamos al servidor para inyectar código PHP. 

Por ejemplo, ponemos en la cabecera de user agent system whoami en una petición web para que quede registrada en el log de apache, y luego leemos `/var/log/apache2/acess.log` y se interpretaría el comándo que hemos puesto en el user agent.

