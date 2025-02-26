# CONFIGURACIONES DE SERVIDORES FTP EN CISCO PAKET TRACER 
# Primer paso

Agregar dispositivos a la hoja de trabajo.Usaremos un servidor,switch y dos pc.

**Seguidamente hacer la conexion entreestos dispositivos:**

<img width="415" alt="image" src="https://github.com/user-attachments/assets/e206977a-55a0-4ded-8002-89ad181e305b" />

Despues asignar una direccion ip y servicios DHCP para que asigne ip automaticamente  a los equipos:

**Direccion ip del servidor**
~~~
192.168.0.3
~~~
**Direccion de inicio ip del DHCP del servidor**

~~~~
192.168.03
~~~~

Desde este punto se asignara ip alos equipos:

# Segundo paso

Verificacion de la conexion entre el servidor y los equipos.
Usaremos el comando :

~~~
ping 
~~~
<img width="509" alt="image" src="https://github.com/user-attachments/assets/408d2753-d6db-4304-ba88-dad0769379d4" />

la conexion entre los equipos fu exitosa.

# Tercer paso

crear y activar cuentas FTP en el servidor y asignar le permisos.

<img width="521" alt="image" src="https://github.com/user-attachments/assets/9dc03fdc-4ade-49dd-b246-533a717f11d2" />

# Cuarto paso

Comprobar conexion FTP en los equipos:

~~~
ftp 192.168.0.3
~~~


<img width="178" alt="image" src="https://github.com/user-attachments/assets/1d643c57-c3c7-436b-9155-1edd35021edd" />

se ingresa la ip del servidor para ver servicios FTP.

# Quinto paso **comandos FTP**
~~~
cd <directorio>	Cambia el directorio en el servidor FTP.
~~~
~~~
delete <archivo>	Elimina un archivo en el servidor FTP (si tiene permisos).
~~~
~~~
dir	Muestra la lista de archivos y carpetas en el servidor FTP.
~~~
~~~
get <archivo>	Descarga un archivo del servidor FTP al dispositivo local.
~~~
~~~
help	Muestra una lista de comandos FTP disponibles y su descripción.
~~~
~~~
passive 	Activa o desactiva el modo pasivo de FTP (usado en firewalls y NAT).
~~~
~~~
put <archivo>	Sube un archivo desde el dispositivo local al servidor FTP.
~~~
~~~
pwd	Muestra el directorio actual en el servidor FTP.
~~~
~~~
quit	Cierra la sesión FTP y regresa al dispositivo.
~~~
~~~
rename <archivo_viejo> <archivo_nuevo>	Cambia el nombre de un archivo en el servidor FTP.
~~~

