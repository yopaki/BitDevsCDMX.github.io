# BitDevs CDMX

Sitio Jekyll sencillo para almacenar todos los enlaces de reuniones pasadas y
futuras.

## Desarrollo 

Es necesario tener instalados [Ruby & Jekyll](https://jekyllrb.com/docs/installation/)
para correr el sitio localmente. Una vez instaladas:

* Clona el repositorio y ve al directorio
* Ejecuta `bundle install`
* Ejecuta `jekyll serve`
* Accede a http://localhost:4000

## Crear una publicación 

Para crear una nueva publicación, crea un archivo nuevo en `_posts/` con el
título `YYYY-MM-DD-el-título-va-aquí`. 
Al comienzo del archivo ingresa la siguiente información:

```md
---
layout: post # Siempre `post`
type: socratic # o `whitepaper` para una serie de white paper
title: "Título de la publicación"
meetup: https://www.meetup.com/BitDevs-CDMX/events/[id del evento]/
---
```

Después usa sencillamente markdown. El sitio autogenerará el resto.

## Cambiar los datos del sitio 

Toda la configuración del sitio esta contenida ya sea en `_config.yml` o en
`_data/settings.yml`. Algunos datos están duplicados entre estos dada la manera
en la que Jekyll inyecta las variables así que asegúrate de actualizar ambos.

## Agradecimientos

Gracias a [LeNPaul](https://github.com/LeNPaul/jekyll-starter-kit) por la
plantilla inicial de Jekyll en la cuál este repositorio de basa.
