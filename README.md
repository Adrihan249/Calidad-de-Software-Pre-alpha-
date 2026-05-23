# Sistema Externo de Monitoreo Web - Etapa 2

Este repositorio contiene el código fuente del panel web externo para el monitoreo de los servicios Passbolt y ChkMonitor mediante SNMP, almacenando los datos en un clúster redundante de MariaDB Galera.

## Estructura del Repositorio
* `server.js`: Servidor Backend en Node.js que expone la API y valida las credenciales.
* `package.json`: Archivo de configuración con las dependencias del proyecto (`express` y `mariadb`).
* `public/index.html`: Interfaz gráfica (Frontend) con login integrado y dashboards en Chart.js.

## Instrucciones de Despliegue en un Servidor Limpio
1. Descargar o clonar esta carpeta en el servidor de monitoreo externo (`192.168.18.26`).
2. Instalar los módulos de Node.js ejecutando en la terminal:
   ```bash
   npm install
3. Iniciar el servidor web de monitoreo:
node server.js
4. Abrir un navegador web en cualquier computadora de la red e ingresar a:
[http://192.168.18.26:3000](http://192.168.18.26:3000)
5. Credenciales de acceso básicas configuradas:
Usuario: admin

Contraseña: admin123
