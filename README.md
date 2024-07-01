# daisyUI-react-doc
Una guía para instalar tailwindcss y daisy UI en React; y no morir en el intento :)



## Paso 1
### instalar tailwindcss
```bash
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```
## Paso 2
### Configura las rutas de tu plantilla ya con daisy

```js
/** @type {import('tailwindcss').Config} */

module.exports = {

  content: [

    "./src/**/*.{js,jsx,ts,tsx}",

  ],

  theme: {

    extend: {},

  },

  plugins: [require('daisyui'),],

}

```

## Paso 3
### Modifica el archivo  `postcss.config.js`

```js
export default {

  plugins: {

    tailwindcss: {},

    autoprefixer: {},

  },

}
```

## Paso 4
### Añade las directivas Tailwind a tu CSS en `./src/index.css`

``` css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

## Paso 5
## Instalar Daisy UI

```
npm i -D daisyui@latest
```

## FIN
