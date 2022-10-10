## Descripción
Este repositorio contiene diferentes archivos flows.json que contienen el código
fuente de distintos flujos de Node-RED.
- horus.json contiene el conector al proyecto Horus del CT Maceira,
- sigefa.json contiene el conector al proyecto SIGEFA del CT Salazar,
- tests.json contiene distintas pruebas de Node-RED.

## Instalación y utilización de Node-RED
1. Clonar este repositorio:
  `git clone https://github.com/fabosso/conectores-api-node-red`
2. Copiar todos los archivos a la carpeta de trabajo de Node-RED.
3. Ingresar a la carpeta de trabajo de Node-RED.
   Por ejemplo, en Windows: C:\Users\NombreDeUsuario\.node-red
4. Instalar dependencias de Node.js:
  `npm install`
5. Renombrar el archivo que corresponda a "flows.json".
6. Lanzar instancia de Node-RED:
  `node-red`

## Notas
- Para abrir el editor de Node-RED: http://127.0.0.1:1880
- En el conector al proyecto Horus es necesario utilizar un broker MQTT para
poder entablecer comunicación con el gateway Dragino. Luego de añadir Mosquitto al PATH:
`mosquitto -c ~/.node-red/mosquitto.conf`
- En el conector al proyecto Horus existe una UI para facilitar el acceso a los comandos
uplink (es decir, comandos que viajan desde el gateway Dragino hacia los nodos). 
Para acceder al mismo: http://127.0.0.1:1880/ui
- En el conector al proyecto SIGEFA se utiliza un nodo de comunicación serial. Si bien
en el mismo se direcciona al COM5, este es representativo del puerto USB con el que se 
comunica al Arduino Nano del nodo interior.
