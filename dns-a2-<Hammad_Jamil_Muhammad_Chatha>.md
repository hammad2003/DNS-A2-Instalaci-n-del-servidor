# Desarrollo de la actividad

##### 1. Configure la máquina virtual con una nueva interfaz en modo puente y con configuración dinámica. Compruebe que puede acceder a la máquina virtual utilizando SSH.

```
```

##### 2. Cambie el hostname de la máquina a dns-a.

```
```

##### 3. Configure la VPN en la máquina virtual.

```
```

##### 4. Compruebe que en la máquina virtual es posible:
- Actualizar la lista de paquetes de los repositorios (apt update)
- Instalar el servidor DNS BIND (apt install bind9)

```
```

##### 5. Conteste a las siguientes preguntas:
- ¿En qué directorio se encuentran los ficheros de configuración de BIND?
- ¿Cuál es fichero de configuración principal?
- ¿Qué ficheros de configuración se incluyen en el fichero de configuración principal?

```
```

##### 6. Arranque el servicio DNS y consulte en el fichero de registro los mensajes de BIND (/var/log/syslog).

```
```

##### 7. Utilice los comandos netstat -putan y ss -na4 para comprobar qué puertos ha abierto BIND.

```
```

##### 8. Realice algunas consultas al servidor DNS:
- ¿Las resuelve? ¿Cómo es posible?
- ¿Cuánto tiempo tarda en resolver un dominio por primera vez?
- ¿Cuánto tiempo tarda en resolver un dominio que ya ha sido resuelto? ¿A qué se debe?
- Ejecute el comando rndc status para obtener información sobre el funcionamiento del servidor.
- Ejecute rndc stats para escribir las estadísticas de uso de BIND9 en /var/cache/bind/named.stats. Consulte las estadísticas generadas.

```
```

##### 9. Cambie la configuración de BIND para que funcione como un servidor de reenvío utilizando el servidor del aula. Arranque el servicio. Compruebe el fichero de registro. Compruebe que BIND funciona como un servidor recursivo para los clientes.
- ¿Cuánto tiempo tarda en resolver un dominio por primera vez?
- ¿Cuánto tiempo tarda en resolver un dominio que ya ha sido resuelto?
- Vuelva a generar el fichero de estadísticas y revise su contenido.

```
```
