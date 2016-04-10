# RedIRIS_edits

[@RedIRIS_edits](https://twitter.com/RedIRIS_edits) es un [Twitterbot](http://en.wikipedia.org/wiki/Twitterbot) que publica los cambios en los artículos de la Wikipedia por usuarios anónimos en la RedIRIS.

[RedIRIS](http://www.rediris.es) es la red académica y de investigación española y proporciona servicios avanzados de comunicaciones a la comunidad científica y universitaria nacional. Está financiada por el Ministerio de Economía y Competitividad, e incluida en su mapa de Instalaciones Científico-Técnicas Singulares (ICTS). Se hace cargo de su gestión la entidad pública empresarial Red.es, del Ministerio de Industria, Energía y Turismo.

RedIRIS cuenta con más de 500 instituciones afiliadas, principalmente universidades y centros públicos de investigación, que llegan a formar parte de esta comunidad mediante la firma de un acuerdo de afiliación.

Este TwitterBot se basa en el proyecto de [edsu/anon](https://github.com/edsu/anon). 

Este proyecto tiene por objeto promover la transparencia en Internet.

## Cómo funciona

El sistema se basa en la evaluación de los canales IRC de Wikipedia, en la que los sistemas de todos los cambios realizados al registro automatizado Wikipedia.

Este flujo de datos [se puede seguir en directo aquí](http://wikistream.wmflabs.org). 

Cualquier cambio que **no se realiza por un usuario registrado** en wikipedia se publicará en Twitter con el siguiente formato:

> _Alguien desde RedIRIS ha editado 'Manel Esteller' en Wikipedia de manera anónima [https://es.wikipedia.org/…](https://es.wikipedia.org/w/index.php?title=Manel_Esteller&curid=4505306&diff=prev&oldid=55426083)_


Las redes de datos son recogidos de diversas fuentes y no pretende ser completa o exactitud. Nos esforzamos por mantener la información actualizada. 

El sistema no hace ninguna evaluación, los datos se procesan directamente. Actualmente no se publicarán todos los cambios marginales con una diferencia de menos de 10 caracteres.

En cuanto a los cambios realizados en Wikipedia, cada cuál deberar juzgar por sí mismo/a.


## Pasadas ediciones en wikipedia

Hemos incluido un fichero que contiene [todas las ediciones realizadas antes de la puesta en marcha de este Bot](blob/master/rediris_parl_wikipedia.md), por usuarios anónimos de Wikipedia desde el rango de IP's de RedIRIS.




