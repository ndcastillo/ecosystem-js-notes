El ecosistema de programación del lenguaje de Javascript es extenso, y se puede separar entre **empaquetadores**, **compiladores**, **frameworks**, **librerías**, **entornos de desarrollo**, **protocolos/arquitecturas de comunicación**, **manejadores de estados** entre otros, aquí se mostraran una clasificación del ecosistema que son mas importantes.

## Module Bundler o Empaquetadores 📦

Los **module bundler** tiene su funcionalidad de empaquetado, **minificación**,  conversión de formatos, test de diagnostico, el **tree shaking**, entre otras utilidades a nuestro proyecto completo. Logrando optimizar y haciendo mas eficiente nuestro código. Existe el caso en solo queremos empaquetar todo nuestro proyecto en un solo archivo, y otras ocaciones dividirlo en partes (chunks) para llamarlo cuando se lo necesite (code splitting). 

Entre las mas populares se encuentran estan **Webpack**, **Parcel**, **Rollup**, **ESBuild** y **Vite ⚡**.

### Webpack (Popularidad y )
Es el empaquetador mas utilizado, su archivo de configuración `webpack.config.js` nos ayudara al momento de describir y configurar como empaquetar nuestros archivos. Nos permite empaquetar desde código en HTML, CSS, Javacript, documentos de preprocesadores, transpiladores, imagenes, iconos, fuentes, y demas archivos estaticos.

Entre sus utilidades se encuentran:

- Gestión de Dependencias
- Ejecución de Tareas
- Conversión de Formatos
- Tener un Servidor de desarrollo

Entre sus grandes ventajas se encuentra su alta configuración, se puede tener un control absoluto de como procesan de los recursos, asi como los sistemas de modularización. 

### Parcel
Parcel es un empaquetador famoso por ser de facil uso, no tiene ningun archivo de configuración, y utilizara su metodología para realizar la empaquetación, donde esta no puede ser configurada y debemos tomar por hecho que fue la mas optima. Su performance en muchas de las veces es sobresaliente, pero en otras ocaciones no es la ideal.

Entre sus utilidades tenemos:
- Gestión de Dependencia
- Ejecución de Tareas
- Tener un Servidor de desarrollo
- Diagnostico
- Tree shaking

### Rollup

Rollup es un empaquetador enfocado en Javacript, nos permite utilizar un archivo de configuración al igual que webpack, pero no realiza un empaquetamiento con otro tipos de archivos que no sea `.js`.

- Ejecución de Tarea
- Tree Shaking
- Empaquetamiento de ES6 y CommonJS modules.

Existen otras tecnologías por ejemplo **ESBuild**, que es una tecnología que tiene un enfoque en JavaScript y que se caracteriza por su velocidad de compilación. En el siguiente [articulo](https://platzi.com/blog/empaquetadores-javascript/) puedes saber aun mas acerca de los empaquetadores.

## Transpiladores
Los Transpiladores son herramientas que **Transforman** y **Compilan** un código y lo convierten 
### Babel
Como sabes a partir de ECMAScript 6, se han seguido actualizando versiones por cada año y añadiendo nuevas funcionalidades, entonces se necesita de una herramienta para poder hacer uso de estas versiones, es por ello que Babel nos permite hacer este cometido.

De esta manera **Babel nos permite utilizar la sintaxis del futuro de Javascript**,
este contendra presets oficiales y otros que puedes crear.
### TypeScript
Es un lenguaje de progrmación tipado y orientado a objetos, donde se puede aprovechar la inyección de dependencias. Entre las ventajas de Typescript es que nos puede ayudar a evitar el envio de errores a producción por ser un lenguaje tipado. Y muchas de las herramientas pueden ser usadas en muchos ambientes.

## Herramientas para UI

En el gran conjunto de herramientas en el frontend se encuentra los frameworks como que tienen un paradigma reactivo y nos permite el manejo de estado de componentes. Entre los mas conocidos se encuentra:

- React
- Vue
- Svelte
- Polymer

## CSS y Preprocesadores

Para la maquetación de cualquier aplicación WEB necesitaremos codificar en CSS, lo podemos hacer con CSS puro, pero existen herramientas como los **preprocesadores** que nos permiten generar pseudocodigo y compilarlo para generar CSS puro, los preprocesadores nos permiten elevar las capacidades del CSS, generar mucho menos codigo repetitivo y llevar una mayor legibidad y orden de nuestro codigo.

Entre los preprocesadores mas conocidos se encuentran:

- SASS
- PostCSS
- Less
- Stylus

Tambien existen preprocesadores para HTML como lo es Pug.

## CSS in JS

En base al concepto de **componente**, podemos agrupar su propia estructura y estilos un solo archivo o en una carpeta completa, y entre las herramientas a utilizar se encuentran:

- Styled Component 
- Emotion 
- JSS
- Glamor

## Herramientas de Enrutamiento
Tambien conocidos como **routers** son aquellos que nos permiten organizar a traves de *query parameters* y rutas de ubicación el contenido de nuestras páginas, los mas conocidos son:

- React Router
- Vue Router
- Svelte Router
- LitElement Router
- Whatever Router

## Frameworks (Todo en uno)
Es un marco de trabajo que contiene muchas de las herramientas anteriormente mencionaadas, y que logra una concistencia unica de dichas herramientas, el usar un framework acelera mucho el desarrollo web. 

Un framework todo en uno es Angular, y levanta una infraestructura grande para realizar su trabajo, pero al ser un marco de trabajo con un conjunto de herramientas seleccionadas, limita y dificulta el uso de otras herramientas que no son compatibles con este framework.

## Entornos de desarrollo (Todo en uno)

Los entornos de desarrollo, que son un grupo de librerias ya configuradas y que trabajan en connjunto, y travez de *CLI* nos permiten realizar diversas configuraciones para implementar rapidamente el desarrollo. Entre los entornos mas conocidos se encuentra:

- Create React App
- Vue CLI
- Svelte CLI
- Polymer CLI
- Whatever CLI

## Manejo de estado
Los manejadores de estados nos facilitan el orden, la **gestión y el control de los estados en los componentes**, a travez de los manejadores podemos centralizar nuestros estados todo nuestro proyecto en un solo lugar.

- Redux
- XSate
- MobX

## Consulta de datos
Para el manejo de datos necesitamos ciertos protocolos de comunicación y herramientas que nos permitan realizar la comunicación entre las bases de datos y nuestro interfaz de usuario. Existen muchas formas de realizarlo, pero las mas conocidas y que hoy en dia son utilizadas son:

- API:REST, se basa en una arquitectura
- GraphQL

Generalmente una aplicación se crea por capas, una capa para el diseño UI/UX y otra capa donde se encuentre la consulta de datos. Existen algunas tecnologías de consulta de datos que nos permiten manejar los estados, como por ejemplo Apolo y nos permiten tener todo en uno.

Lo que se ha realizado es un vistado general del ecosistema de JavaScript, existen muchisimas pero muchisimas mas tecnologías basadas en JavaScript, pero las mas básicas y mas utilizadas a hoy por hoy son listadas anteriormente.
**Contribución realizada por:** David Castillo