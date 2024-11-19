# Ejercicio 1: Despliegue del Tema "minima" en GitHub Pages

Este documento describe los pasos necesarios para desplegar un sitio Jekyll utilizando el tema "minima" en GitHub Pages. Primero se configurará el sitio en local y luego se desplegará en GitHub Pages.

---

## Paso 1: Instalación de Jekyll

Para desplegar el tema "minima" en GitHub Pages, primero instalaremos Jekyll en tu sistema.

1. Asegúrate de tener **Ruby** y **RubyGems** instalados.
2. Abre una terminal y ejecuta el siguiente comando para instalar Jekyll y Bundler:
   ```
   gem install jekyll bundler
   

## Paso 2: Crear un Nuevo Sitio Jekyll
Crea un nuevo proyecto de Jekyll utilizando el tema "minima":
```
jekyll new myblog --force --skip-bundle
cd myblog
```
Una vez creado el proyecto, abre el archivo _config.yml y edítalo para personalizar los datos del blog:
```
title: "Mi Blog Personal"
author: "Tu Nombre y Apellido"
email: "tuemail@ejemplo.com"
```
## Paso 3: Personalización del Blog
## Modificar las Páginas por Defecto
Abre los archivos index.markdown y about.markdown que vienen en el directorio raíz.
Cambia el contenido de estas páginas para personalizarlas de acuerdo con la temática del blog que has elegido.
## Crear una Nueva Página
Copia el archivo index.markdown o crea uno nuevo, por ejemplo, contact.markdown, y añade contenido personalizado.
Dale un nombre que describa la nueva página y su contenido.

## Paso 4: Añadir Publicaciones
Para añadir contenido a tu blog, crea al menos tres publicaciones en la carpeta _posts siguiendo la convención de nombres yyyy-mm-dd-nombre-del-post.markdown. A continuación, tienes un ejemplo de cómo puede verse el contenido de una publicación:
```
---
layout: post
title: "Bienvenidos a Mi Blog"
date: 2024-10-22
---
¡Hola! Esta es mi primera publicación en mi blog Jekyll. Aquí hablaré sobre [tu temática].
```

## Paso 5: Ejecutar el Sitio en Local
Antes de subir el sitio, pruébalo en tu servidor local para ver cómo se visualiza.
Ejecuta el siguiente comando en tu terminal:
```
bundle exec jekyll serve
```
Accede a http://localhost:4000 en tu navegador para visualizar el sitio en local.

## Paso 6: Configurar GitHub Pages
Subir a GitHub
Crea un repositorio en GitHub con el nombre myblog.

En tu terminal, vincula el repositorio local al repositorio de GitHub y sube los archivos:

```
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/tu_cuenta/myblog.git
git push -u origin main
```
## Activar GitHub Pages
Entra en la configuración del repositorio en GitHub.
Activa GitHub Pages seleccionando la rama main como fuente de publicación.