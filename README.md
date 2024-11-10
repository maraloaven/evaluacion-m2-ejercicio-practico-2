
# Ejercicio 2 - Página Web Clínica con HTML, CSS y SASS

Este es un proyecto de una página web para la Clínica Clínica, diseñado con HTML y CSS (SASS). El sitio web presenta información básica de la clínica, incluyendo una página de bienvenida, detalles sobre el equipo médico y una sección de contacto.

## Descripción del Proyecto

La página web de la Clínica consta de tres secciones principales:

**1. Página de Bienvenida (index.html):** Página de bienvenida que incluye una introducción al hospital, un apartado sobre los servicios que ofrece y una sección de testimonios de pacientes, proporcionando confianza a los nuevos visitantes.

**2. Equipo Médico (equipo-medico.html):** Página que muestra el equipo médico con una foto de cada uno, una breve descripción de cada miembro y su especialidad.

**3. Contacto (contacto.html):** Página de contacto con un formulario para que los usuarios puedan enviar mensajes y un mapa interactivo que muestra la ubicación del hospital.

**4. Barra de Navegación (custom_navbar.html):** Es un elemento extra presente en todas las vistas, para mostrar una barra de navegación.

#### Tecnologías utilizadas
- HTML
- CSS
- SASS
- Media Query

# Proyecto de Estilos Responsivos con SASS

Este proyecto tiene como objetivo crear un diseño responsivo para una página web utilizando SASS para la modularización de los estilos. Se implementan media queries para asegurar que el diseño se adapte correctamente a diferentes tamaños de pantalla.

## Modularización de los Estilos y Media Queries

Para mantener el código limpio y organizado, se implementó la **modularización de los estilos** usando SASS. Esto permitió dividir los estilos en archivos parciales reutilizables.

### Media Queries

Las media queries están basadas en los siguientes puntos de interrupción (breakpoints):

- **punto de quiebre pequeño:** 768px
- **punto de quiebre mediano:** 769px - 1024px
- **punto de quiebre grande:** 1024px

Se implementaron en diversas secciones del proyecto para hacer que los elementos del diseño se ajusten de manera fluida dependiendo del tamaño de la pantalla:

- Para pantallas pequeñas (menos de 768px), se usan modificaciones como cambiar la orientación de los elementos de fila a columna, reducir tamaños de letras, etc.
- Para pantallas medianas (entre 769px y 1023px), se ajustan los tamaños de las fuentes.
- Para pantallas grandes (mayores de 1024px), se aplica un diseño más amplio y espacioso.

### Estructura de los Archivos SASS

La estructura de los archivos SASS y del proyecto en general está organizada de la siguiente manera para promover la reutilización y facilitar el mantenimiento:


        /evaluacion-m2-ejercicio-practico-2
        │
        ├── index.html                
        ├── equipo-medico.html         
        ├── contacto.html         
        ├── custom_navbar.html         
        │
        ├── scss/
        │   ├── main.scss
        │   ├── main.css 
        │   ├── main.css.map
        │   ├── abstracts
        │   │   └── _variables-mixins.scss
        │   ├── base
        │   │   └── _base.scss
        │   ├── components
        │   │   └── _navbar.scss
        │   ├── layout
        │   │   └── _header-footer.scss
        │   ├── pages
        │   │   └── _home.scss
        │   ├── themes
        │   │   └── _helpers.scss
        │
        ├── img/                  
        │    ├── dr1.jpg
        │    ├── dr2.jpg
        │    ├── dr3.jpg
        │    ├── dr4.jpg 
        │    ├── logo.jpg      
        │    ├── pac1.jpg   
        │    ├── pac2.jpg    
        │    ├── pac3.jpg  
        │    ├── ser1.jpg 
        │    ├── ser2.jpg    
        │    └── ser3.jpg           
        │
        ├── node_modules
        ├── .gitignore
        ├── package-lock.json
        ├── package.json
        └── README.md                 

### Aplicación de la metodología BEM (Bloques, Elementos, Modificadores)

Para mantener el código CSS bien estructurado y fácil de mantener, se utilizó la **metodología BEM** en la creación de clases CSS. Esto asegura que las clases sean descriptivas y que los componentes sean modulares y reutilizables.

- **Bloques:** Son las secciones principales del diseño, como `.navbar`, `.hero`, `.contact`, etc.
- **Elementos:** Son los componentes dentro de los bloques, como `.navbar__link`, `.hero__title`, etc.
- **Modificadores:** Son los elementos que fueron modificados, como `.navbar__link--special`.


## Instrucciones para Visualizar el Proyecto

### Requisitos Previos

- Tener **Node.js** y **npm** instalados.
- Tener **SASS** instalado globalmente. Puede instalarse ejecutando el siguiente comando:

        npm install -g sass

### Pasos para Ejecutar el Proyecto

1. Clona el repositorio en tu máquina local:

        git clone <URL del repositorio>
        cd <nombre del repositorio>
2. Instala las dependencias necesarias (si es que usas alguna para el proyecto).

3. Compila los archivos SASS en CSS ejecutando el siguiente comando:

        sass scss/main.scss:scss/main.css
4. Abre el archivo `index.html` (o cualquier otro archivo HTML del proyecto) en tu navegador:
- Utiliza Live Server (si estás trabajando en VS Code) para ver la página en tu navegador
- Haz clic derecho sobre `index.html`.
- Selecciona "Open with Live Server" para iniciar la página en tu navegador.

## Autor

- Martín Avendaño.