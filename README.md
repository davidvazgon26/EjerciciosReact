# EjerciciosReact


## Inicio de instrucciones para ejercicio " Interfaz2doCurso "

https://raybo.org/slides_reactinterface/#/

## Para instalar react-icons:

npm install react-icons --save

Esto es para usar el framework de iconos en lugar de estar trabajando con imagenes y sus rutas

Los iconos disponibles los puedes encontrar en el siguiente  [enlace](https://react-icons.github.io/react-icons)

## Instalar Tailwind

npm install -D tailwindcss@npm:@tailwindcss/postcss7-compat @tailwindcss/postcss7-compat postcss@^7 autoprefixer@^9 @tailwindcss/forms

## Instalar craco

npm install @craco/craco

Agregar a nuestro package json en la parte de scripts:

"start": "craco start"
"build": "craco build"
"test": "craco test"

## Crear archivo de configuracion para craco
En la raiz crear craco.config.js y pegar el siguiente codigo:

//craco.config.js

`
module.exports ={
    style:{
        postcss:{
            plugins:[
                require('tailwindcss'),
                require('autoprefixer'),
            ],
        },
    },
}
`

## Instalar o inicializar configurador de Tailwind

npx tailwindcss init    

Para inicializar nuestro archivo tailwind.config.js, donde insertaremos el siguiente codigo:

`
module.exports = {
  purge: ['./src/**/*.{js,jsx,ts,tsx}','./public/index.html'],
  darkMode: false, // or 'media' or 'class'
  theme: {
    extend: {},
  },
  variants: {
    extend: {},
  },
  plugins: [require('@tailwindcss/forms')],
}
`

## Modificar nuestro CSs

Necesitamos insertar o reemplazar el siguiente codigo en el archivo index.css

@tailwind base;
@tailwind components;
@tailwind utilities;

## Podemos comenzar a aplicar los estilos de tailwind

por ejemplo podemos usar container en App.js



## Fin de instrucciones para ejercicio " Interfaz2doCurso "
