#Cheatsheet #Ffuf

| **Dominio**                                                                                                                                                     | **Descripción**              |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------- |
| `ffuf -h`                                                                                                                                                       | ffuf ayuda                   |
| `ffuf -w wordlist.txt:FUZZ -u http://SERVER_IP:PORT/FUZZ`                                                                                                       | Fuzzing de directorios       |
| `ffuf -w wordlist.txt:FUZZ -u http://SERVER_IP:PORT/indexFUZZ`                                                                                                  | Fuzzing de extensión         |
| `ffuf -w wordlist.txt:FUZZ -u http://SERVER_IP:PORT/blog/FUZZ.php`                                                                                              | Fuzzing de página            |
| `ffuf -w wordlist.txt:FUZZ -u http://SERVER_IP:PORT/FUZZ -recursion -recursion-depth 1 -e .php -v`                                                              | Fuzzing recursivo            |
| `ffuf -w wordlist.txt:FUZZ -u https://FUZZ.hackthebox.eu/`                                                                                                      | Fuzzing de subdominios       |
| `ffuf -w wordlist.txt:FUZZ -u http://academy.htb:PORT/ -H 'Host: FUZZ.academy.htb' -fs xxx`                                                                     | Fuzzing de VHost             |
| `ffuf -w wordlist.txt:FUZZ -u http://admin.academy.htb:PORT/admin/admin.php?FUZZ=key -fs xxx`                                                                   | Fuzzing de parámetros - GET  |
| `ffuf -w wordlist.txt:FUZZ -u http://admin.academy.htb:PORT/admin/admin.php -X POST -d 'FUZZ=key' -H 'Content-Type: application/x-www-form-urlencoded' -fs xxx` | Fuzzing de parámetros - POST |
| `ffuf -w ids.txt:FUZZ -u http://admin.academy.htb:PORT/admin/admin.php -X POST -d 'id=FUZZ' -H 'Content-Type: application/x-www-form-urlencoded' -fs xxx`       | Fuzzing de valores           |

# Listas de palabras

|**Dominio**|**Descripción**|
|---|---|
|`/opt/useful/SecLists/Discovery/Web-Content/directory-list-2.3-small.txt`|Directorio/Página Lista de palabras|
|`/opt/useful/SecLists/Discovery/Web-Content/web-extensions.txt`|Lista de palabras de extensiones|
|`/opt/useful/SecLists/Discovery/DNS/subdomains-top1million-5000.txt`|Lista de palabras de dominio|
|`/opt/useful/SecLists/Discovery/Web-Content/burp-parameter-names.txt`|Lista de palabras de parámetros|

# Varios

| **Dominio**                                                                                                                   | **Descripción**                      |
| ----------------------------------------------------------------------------------------------------------------------------- | ------------------------------------ |
| `sudo sh -c 'echo "SERVER_IP academy.htb" >> /etc/hosts'`                                                                     | Agregar entrada DNS                  |
| `for i in $(seq 1 1000); do echo $i >> ids.txt; done`                                                                         | Crear lista de palabras de secuencia |
| `curl http://admin.academy.htb:PORT/admin/admin.php -X POST -d 'id=key' -H 'Content-Type: application/x-www-form-urlencoded'` | ffuf con POST                        |
