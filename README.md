# El Hombre Tecnológico

Biblioteca visual de Tecnología e Informática conectada con [tu blog](https://elhombretecnologico.blogspot.com/). Está pensada para que el alumnado encuentre recursos por tema y para que puedas añadir nuevas entradas y vídeos desde Blogger.

## Cómo añadir contenido

La forma más sencilla es seguir usando Blogger:

1. Entra en [Blogger](https://www.blogger.com/) y crea una entrada nueva.
2. Escribe un título claro, una explicación corta y añade la etiqueta Portada para que aparezca en la web. Puedes añadir otras etiquetas como Tecnología, Informática, GIMP o Robótica.
3. Para añadir un vídeo, pulsa **Insertar vídeo → Subir desde el ordenador**. No hace falta usar YouTube.
4. Publica la entrada. La portada de esta web recoge automáticamente las últimas publicaciones del blog.

El blog tiene que mantener activo el feed de entradas. Ahora mismo está activo. Si alguna vez dejas de ver las novedades, revisa **Blogger → Configuración → Feed del sitio → Permitir feed**. Solo aparecen en esta web las entradas marcadas como Portada.

## Recursos destacados que ya están en la web

- Electrónica digital: vídeo sobre XOR, apuntes EBAU, mapas de Karnaugh y soluciones.
- Neumática: ficha de bachillerato.
- GIMP: vídeo de retoque y práctica guiada.
- Informática: ficha de hardware y software.
- Tecnología: ficha de tangram para construcción.
- Diseño: apuntes de diseño asistido por ordenador.

Los archivos están dentro de recursos/. No se han copiado trabajos de alumnos, nombres de estudiantes ni documentos administrativos.

## Añadir un archivo seleccionado

Si quieres que un PDF o vídeo pequeño aparezca como recurso destacado:

1. Copia el archivo en una subcarpeta de recursos/.
2. Añade una tarjeta con su título, área, descripción y ruta en contenido.json.
3. Sube el cambio al repositorio para que la web se actualice.

Cloudflare Pages limita cada archivo estático a 25 MiB. Para vídeos grandes, usa la opción de subida directa de vídeo de Blogger. [Límites de Cloudflare Pages](https://developers.cloudflare.com/pages/platform/limits/) · [Ayuda de Blogger para vídeos](https://support.google.com/blogger/answer/41641?hl=es)

## Publicación gratuita

- **GitHub** guarda el código.
- **Cloudflare Pages** publica la web y permite conectarse a un repositorio privado.
- **Blogger** sirve para añadir entradas y vídeos desde una interfaz que ya conoces.

En Cloudflare, selecciona **Workers & Pages → Create application → Pages → Connect to Git**, conecta el repositorio y publica la rama main. Configura el comando de compilación como:

    mkdir -p public && cp index.html app.js styles.css contenido.json favicon.svg public/ && cp -r recursos public/

Usa public como carpeta de salida. No hace falta framework ni base de datos. La web y sus materiales destacados serán públicos para que el alumnado pueda consultarlos.

Como alternativa, puedes activar GitHub Pages con **Settings → Pages → GitHub Actions**. El repositorio tendrá que ser público en GitHub Free; Cloudflare Pages admite repositorios privados y públicos.

## Selección de D:\INSTI

La carpeta completa supera el espacio razonable para una web gratuita, así que he empezado con una selección de recursos didácticos pequeños. Se dejan fuera trabajos individuales, carpetas con nombres de alumnado, documentos del centro, instaladores y archivos personales. Los materiales se pueden ampliar poco a poco, según los vayas necesitando.
