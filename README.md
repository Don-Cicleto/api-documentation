# DON CICLETO API DOCUMENTATION

## Introducción
En este documento, encontrarás instrucciones detalladas sobre cómo publicar la documentación de API Blueprint (.apib) en GitHub Pages.

## Requisitos previos
Antes de comenzar, asegúrate de tener lo siguiente:
- Una cuenta de GitHub.
- Git instalado en tu máquina local.
- El archivo `.apib` de tu proyecto de API Blueprint listo para ser publicado.

## Instalación y configuración de herramientas necesarias
Para convertir tu archivo `.apib` en HTML, utilizaremos Aglio, una herramienta de línea de comandos. Para instalar Aglio, necesitarás Node.js y NPM. Sigue estos pasos:

1. Instala Node.js y NPM: Visita https://nodejs.org/ y descarga la versión recomendada para tu sistema operativo. La instalación de Node.js incluye NPM.
2. Instala Aglio: Abre una terminal y ejecuta el siguiente comando:

```bash
npm install -g aglio
```

## Generación de la documentación HTML a partir del archivo .apib
Una vez instalado Aglio, puedes generar un archivo HTML a partir de tu archivo `.apib` utilizando el siguiente comando:

```bash
aglio -i doncicleto.apib -o index.html
```

Esto convertirá tu archivo `.apib` en un archivo `index.html` que puedes publicar en GitHub Pages.

## Configuración de GitHub Pages para el proyecto
Para configurar GitHub Pages, sigue estos pasos:
1. Ve al repositorio de tu proyecto en GitHub.
2. Haz clic en la pestaña "Settings" (Configuración).
3. Desplázate hasta la sección "GitHub Pages".
4. Selecciona la rama desde la cual quieres publicar tu sitio (por ejemplo, `main` o `gh-pages`).
5. Haz clic en "Save" (Guardar).

## Publicación de la documentación en GitHub Pages
Para publicar tu documentación:
1. Añade el archivo `index.html` a tu repositorio git si aún no lo has hecho:

```bash
git add index.html
git commit -m "Añade documentación de API Blueprint"
git push
```

2. Sigue los pasos en la sección anterior para configurar GitHub Pages.
3. Una vez configurado, tu documentación estará disponible en la URL proporcionada por GitHub Pages.

## Actualización de la documentación
Para actualizar tu documentación, simplemente genera de nuevo el archivo `index.html` con Aglio cada vez que hagas cambios en tu archivo `.apib` y sube los cambios a tu repositorio de GitHub.
