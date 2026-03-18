# Daniel-Gorras-Cristianas

Sitio BOON & BLESS convertido a proyecto Node.js con Express para despliegue en Hostinger.

## Estructura

- `server.js`: servidor Express.
- `public/`: web estatica (HTML + imagenes).
- `package.json`: scripts y dependencias.

## Ejecutar en local

1. Instala dependencias:

	npm install

2. Inicia el servidor:

	npm start

3. Abre en navegador:

	http://localhost:3000

## Deploy en Hostinger (Node.js)

1. Sube todos los archivos del proyecto (incluyendo `public/`, `server.js`, `package.json`).
2. En el panel de Node.js de Hostinger, configura:
	- Versión de Node: 18 o superior.
	- Startup file: `server.js`.
	- Comando de inicio: `npm start`.
3. Ejecuta instalación de dependencias:

	npm install --production

4. Reinicia la app desde el panel.
5. Verifica que tu dominio apunte a la aplicación Node (segun la configuracion del panel).

## Variables de entorno

- `PORT`: Hostinger lo asigna automaticamente en la mayoria de entornos. El servidor ya lo soporta con `process.env.PORT`.

## Nota

Si tu plan no incluye soporte para Node.js, debes usar un plan con Node habilitado o VPS.