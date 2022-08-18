## Instalación y utilización de Node-RED
1. Clonar este repositorio:
  `git clone https://github.com/fabosso/conectores-api-node-red`
2. Copiar todos los archivos a la carpeta de trabajo de Node-RED:
  `cp -i conectores-api-node-red/. ~/.node-red`
3. Ingresar a la carpeta de trabajo de Node-RED:
  `cd ~/.node-red`
 4. Instalar dependencias de Node.js:
  `npm install`
 5. Lanzar instancia de Node-RED:
  `node-red`

## Utilización de Mosquitto
Luego de añadir Mosquitto al PATH:
`mosquitto -c ~/.node-red/mosquitto.conf`