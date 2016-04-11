# RedIRIS_edits

[@RedIRIS_edits](https://twitter.com/RedIRIS_edits) es un [Twitterbot](http://en.wikipedia.org/wiki/Twitterbot) que publica los cambios realizados en la Wikipedia por usuarios anónimos desde la RedIRIS.

La [RedIRIS](http://www.rediris.es) es la red académica y de investigación española y proporciona servicios avanzados de comunicaciones a la comunidad científica y universitaria nacional. 

RedIRIS cuenta con más de 500 instituciones afiliadas, principalmente universidades y centros públicos de investigación.

Este TwitterBot se basa en el proyecto de [edsu/anon](https://github.com/edsu/anon) y su objetivo es promover la transparencia en Internet.


## Cómo funciona

El sistema se basa en la evaluación de los canales IRC de Wikipedia, en la que los sistemas de todos los cambios realizados al registro automatizado Wikipedia.

Este flujo de datos [se puede seguir en directo aquí](http://wikistream.wmflabs.org). 

Cualquier cambio que **no se realiza por un usuario registrado** en wikipedia se publicará en Twitter con el siguiente formato:

> _Alguien desde RedIRIS ha editado 'Manel Esteller' en Wikipedia de manera anónima [https://es.wikipedia.org/…](https://es.wikipedia.org/w/index.php?title=Manel_Esteller&curid=4505306&diff=prev&oldid=55426083)_

Las redes de datos son obtenidas de diversas fuentes y no pretende ser completa o exactitud. Nos esforzamos por mantener la información actualizada. Puedes proponer los cambios que consideres oportunos enviando una solicitud a este repositorio.

El rango de direcciones empleado [lo encontrarás en el siguiente archivo](rediris-networks.json). 

El sistema no hace ninguna evaluación, los datos se procesan directamente. Actualmente no se publicarán todos los cambios marginales con una diferencia de menos de 10 caracteres.

En cuanto a los cambios realizados en Wikipedia, cada cuál deberar juzgar por sí mismo/a.


## Pasadas ediciones en wikipedia desde RedIRIS

Hemos incluido un fichero que contiene [todas las ediciones realizadas antes de la puesta en marcha de este Bot](rediris_parl_wikipedia.md), por usuarios anónimos de Wikipedia desde el rango de IP's de RedIRIS.




