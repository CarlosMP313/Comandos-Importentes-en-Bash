# Comandos Importantes de Bash para Especialistas en Kali Linux

## 1. Navegación y Gestión de Archivos

- **`ls`**: Lista los archivos y directorios en el directorio actual.
```bash
  ls -la
```
- **`l`**: Muestra la lista en formato largo.
```bash
  ls -l
```
- **`a`**: Incluye archivos ocultos.
```bash
  ls -a
```
- **`cd`**: Cambia el directorio actual.
```bash
  cd /ruta/del/directorio
```

- **`cp`**: Copia archivos o directorios.
```bash
  cp archivo_origen archivo_destino
```

- **`r`**: Copia recursivamente (para directorios).
```bash
  cp -r archivo_origen archivo_destino
```
  
- **`mv`**: Mueve o renombra archivos o directorios.
```bash
  mv archivo_origen archivo_destino
```

- **`rm`**: Elimina archivos o directorios.
```bash
  rm archivo
```

-**`r`**: Elimina recursivamente (para directorios).
```bash
  rm -r archivo
```

-**`f`**: Fuerza la eliminación sin preguntar.
```bash
  rm -f archivo
```
-**`mkdir`**: Crea un nuevo directorio.
```bash
  mkdir nombre_del_directorio
```

- **`touch`**: Crea un archivo vacío o actualiza la fecha de modificación de un archivo existente.
```bash
  touch nombre_del_archivo
```

## 2. Permisos y Propiedades
chmod: Cambia los permisos de archivos o directorios.

bash
Copiar código
chmod 755 archivo
755: Permisos de lectura y ejecución para todos, escritura solo para el propietario.
chown: Cambia el propietario de un archivo o directorio.

bash
Copiar código
chown usuario:grupo archivo
3. Gestión de Procesos
ps: Muestra los procesos en ejecución.

bash
Copiar código
ps aux
a: Muestra todos los procesos de todos los usuarios.
u: Muestra el propietario del proceso.
x: Incluye procesos sin terminal asociado.
top: Monitorea los procesos en tiempo real.

bash
Copiar código
top
kill: Termina un proceso mediante su ID (PID).

bash
Copiar código
kill -9 PID
-9: Señal de terminación forzada.
pkill: Termina procesos por nombre.

bash
Copiar código
pkill nombre_proceso
4. Red y Conectividad
ifconfig: Muestra o configura las interfaces de red.

bash
Copiar código
ifconfig
ping: Verifica la conectividad con un host.

bash
Copiar código
ping ejemplo.com
netstat: Muestra las conexiones de red y estadísticas de red.

bash
Copiar código
netstat -tuln
-t: Conexiones TCP.
-u: Conexiones UDP.
-l: Solo conexiones en escucha.
-n: Muestra direcciones numéricas.
nmap: Escanea redes y puertos.

bash
Copiar código
nmap -sS -p- ejemplo.com
-sS: Escaneo SYN (rápido).
-p-: Escanea todos los puertos.
5. Administración de Paquetes
apt: Gestiona paquetes en sistemas basados en Debian.

bash
Copiar código
sudo apt update && sudo apt upgrade
update: Actualiza la lista de paquetes.
upgrade: Actualiza los paquetes instalados.
dpkg: Gestiona paquetes Debian.

bash
Copiar código
dpkg -i paquete.deb
6. Búsqueda y Manipulación de Texto
grep: Busca patrones en archivos o entrada.

bash
Copiar código
grep "patrón" archivo
awk: Procesa y analiza texto basado en patrones.

bash
Copiar código
awk '{print $1}' archivo
sed: Edita texto de forma automática en flujo.

bash
Copiar código
sed 's/original/nuevo/g' archivo
7. Compresión y Archivos
tar: Archiva y descomprime archivos tar.

bash
Copiar código
tar -czvf archivo.tar.gz directorio
-c: Crea un archivo.
-z: Comprime con gzip.
-v: Muestra el progreso.
-f: Especifica el nombre del archivo.
unzip: Descomprime archivos zip.

bash
Copiar código
unzip archivo.zip
8. Comandos Especiales de Kali Linux
msfconsole: Inicia Metasploit Framework.

bash
Copiar código
msfconsole
hydra: Herramienta de fuerza bruta para ataques a contraseñas.

bash
Copiar código
hydra -l usuario -P lista_passwords ssh://objetivo
nikto: Escáner de vulnerabilidades para servidores web.

bash
Copiar código
nikto -h http://objetivo.com
9. Alias y Scripts
alias: Define comandos personalizados.

bash
Copiar código
alias actualizar='sudo apt update && sudo apt upgrade'
bash script.sh: Ejecuta un script Bash.

bash
Copiar código
./script.sh
10. Otros Comandos Útiles
history: Muestra el historial de comandos ejecutados.

bash
Copiar código
history
crontab: Administra tareas programadas.

bash
Copiar código
crontab -e
man: Muestra el manual de un comando.

bash
Copiar código
man comando

