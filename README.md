# RedIRIS_edits

[@RedIRIS_edits](https://twitter.com/RedIRIS_edits) es un [Twitterbot](http://en.wikipedia.org/wiki/Twitterbot) que publica los cambios realizados en la Wikipedia por usuarios anónimos desde la RedIRIS.

La [RedIRIS](http://www.rediris.es) es la red académica y de investigación española y proporciona servicios avanzados de comunicaciones a la comunidad científica y universitaria nacional. 

RedIRIS cuenta con más de 500 instituciones afiliadas, principalmente universidades y centros públicos de investigación.

Este TwitterBot se basa en el proyecto de [edsu/anon](https://github.com/edsu/anon) y su objetivo es promover la transparencia en Internet.


## El TwitterBot

Este bot opera en twitter con el nick [@SpainGovedits](https://twitter.com/SpainGovedits) desde abril de 2016.

	El pasado 28 de marzo de 2018 se decidió dar de baja por motivos de espacio 
	y de poco interés en las ediciones detectadas.

[En este enlace](twitter/719199624989446144_ec33d20b55fcd7037c23137d0a8e4fbc159a6dff.zip) se puede descargar el zip con todos los posts de la cuenta.

En carpeta /twitter se puede encontrar el código empleado por el bot basado en el proyecto [edsu/anon](https://github.com/edsu/anon), así como las imágenes de la identidad de twitter.

> @RedIRIS_edits
> Tuitea las ediciones anónimas en Wikipedia desde el rango de IP's de RedIRIS,   
> la red de comunicaciones para la comunidad científica y universitaria española.


## Cómo funciona

El sistema se basa en la evaluación de los canales IRC de Wikipedia, en los que todos los cambios realizados a páginas de la wikipedia son automáticamente registrados.

Para haceros una idea de este flujo de datos [podeis seguir en directo](http://wikistream.wmflabs.org) una muestra creado por el [Wikimedia Tool Labs](http://tools.wmflabs.org/).

Cualquier cambio que **no se realiza por un usuario registrado** en wikipedia se publicará en Twitter con el siguiente formato:

> _Alguien desde RedIRIS ha editado 'Manel Esteller' en Wikipedia de manera anónima [https://es.wikipedia.org/…](https://es.wikipedia.org/w/index.php?title=Manel_Esteller&curid=4505306&diff=prev&oldid=55426083)_

## Rangos de IP

Las redes de datos son obtenidas de diversas fuentes y no pretende ser completa o exactitud. Nos esforzamos por mantener la información actualizada. Puedes proponer los cambios que consideres oportunos enviando una solicitud a este repositorio.

El rango de direcciones empleado [lo encontrarás en el siguiente archivo](rediris-networks.json). 

Este rango no está categorizado de ninguna manera, ( es decir por Universidad o centro específico), cosa que lo haría más interesante. :)

El sistema no hace ninguna evaluación, los datos se procesan directamente. Actualmente no se publicarán todos los cambios marginales con una diferencia de menos de 10 caracteres.

En cuanto a los cambios realizados en Wikipedia, cada cuál deberar juzgar por sí mismo/a.


## Pasadas ediciones en wikipedia desde RedIRIS

Hemos incluido un fichero que contiene [todas las ediciones realizadas antes de la puesta en marcha de este Bot](rediris_parl_wikipedia.md), por usuarios anónimos de Wikipedia desde el rango de IP's de RedIRIS.




