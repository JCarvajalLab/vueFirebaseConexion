# vueFirebaseConexion
Vamos a registrar los pasos para conectar un proyecto vue a firebase validar una url

## PASOS PARA AGREGAR UN PROYECTO VUE Y SUBIRLO A GITHUB PAGE

- Paso 1. Crear proyecto de VUE CLI (Agregar vuex/router si es necesario)

- Paso 3. Agregar la siguiente linea de comando a vue.config.js (El proyecto actual es VUE 3)

```javascript
module.exports = defineConfig({
  transpileDependencies: true,
  publicPath: process.env.NODE_ENV === 'production' ? '/gitpagepruebafinal3/' : '/'
})
```
>[!IMPORTANT]
>Debemos modificar la ruta y agregar la del github, yo realice una prueba en el cual eran diferentes y no me funcionaba
>
- Se comienza a realizar la instalacion de FIREBASE
npm install -g firebase-tools

- el npm run build para crear la carpeta dist

npm run build

Luego se de realizar la instalacion debemos iniciar secion con FIREBASE

firebase login

Ahora crearemos las iniciaremos el firebase con 

firebase init

-Are you ready to proceed? Yes
-Which Firebase features do you want to set up for this directory? Press Space to select features, then Enter to confirm your choices. Hosting: Configure files for Firebase Hosting and (optionally) set up GitHub Action deploys
-Please select an option: Use an existing project
-Select a default Firebase project for this directory: conexionfirebases-70658 (conexionfirebases) [seleccionamos el proyecto creado]
-What do you want to use as your public directory? dis
-Configure as a single-page app (rewrite all urls to /index.html)? Yes
- Set up automatic builds and deploys with GitHub? (y/N) [esta opcion es opcional, vamos a probar sin seleccionarla]
- Set up automatic builds and deploys with GitHub? No
- -File dist/index.html already exists. Overwrite? No

Ahora utilizamos el firebase deploy para 

