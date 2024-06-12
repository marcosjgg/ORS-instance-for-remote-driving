# ORS-instance-for-remote-driving

montado en la máquina virtual proporcionada por ETSIT-UPM
VNX
modificar VNX a 3 servidores en la misma red:
1- ORS
2- Route Scheduler
3- Remote Driver

instalar ORS en el servidor ORS, siguiendo las indicaciones de la pagina web para Build from source code
--modificar archivos de ORS para cargar mapa de Madrid
---paso de pruebas--- hacer los 4 scripts (ruta simple, multiples rutas, avoid areas, añadir paradas en el trayecto)
montar en route_scheduler un servidor Fast-API para leer rutas desde ORS que sean pedidas desde Remote Driver
realizar peticiones curl a route_scheduler desde remote_driver
-----------------por hacer--------------
hacer que el servidor fastApi sea capaz de procesar varias peticiones a la vez
en el script de main.py en route_scheduler hay que implementar las 4 funcionalidades que se piden (no me sale). Si quito avoid_polygons de la funcion principal no me funciona el programa
