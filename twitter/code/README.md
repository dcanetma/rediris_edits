# RedIRIS_anon

This bot will watch wikipedia edits from the IP range used by the RedIris Intranet proxies and will tweet (in spanish) when it notices one.  

It was inspired by
[@parliamentedits](https://twitter.com/parliamentedits) and is used to make
[@congressedits](https://twitter.com/congressedits) available. It is now being
used a [community](#community) of users to post selected Wikipedia edits to 
Twitter.

#### Formato del mensaje

> Alguien desde RedIRIS ha editado 'Manel Esteller' en Wikipedia de manera anónima https://es.wikipedia.org/w/index.php?title=Manel_Esteller&curid=4505306&diff=prev&oldid=55426083

#### About RedIris

> _"Connecting the spanish R+D+i since 1988"_

[RedIRIS](http://www.rediris.es/) is the Spanish academic and research network that provides advanced communication services to the scientific community and national universities. It is funded by the Ministry of Economy and Competitiveness and is included in the Ministry's map of Special Scientific and Technological Facilities (ICTS). It is managed by the Public Corporate Entity Red.es, which reports to the Ministry of Industry, Energy and Tourism.

RedIRIS has over 500 affiliated institutions, mainly universities and public research centres, which join this community by signing an affiliation agreement.

You can view detailed information about RedIRIS and its main lines of action: 

- [Brochure](http://www.rediris.es/rediris/mm/diptico_rediris_2012.pdf)
- [Presentation](http://www.rediris.es/rediris/mm/RedIRIS_corporate-presentation.pdf)

## Run

To run anon you will need to:

1. install [Node](http://nodejs.org)
1. `npm install -g coffee-script`
1. `git clone https://github.com/edsu/anon.git`
1. `cd anon`
1. `npm install`
1. `cp config.json.template config.json`
1. add twitter credentials for your bot to `config.json` (make sure the Twitter
app you create has read/write permission so it can tweet)
1. add IP ranges/names to `config.json`
1. modify status template if desired
1. `./anon.coffee` 



### IP Ranges

Using domaintools.com we get the ip address for the web server of the main domain 'rediris.es'

- http://reverseip.domaintools.com/search/?q=rediris.es

Resulting on the IP **130.206.13.20** that we use [to query on RIPE's database](https://apps.db.ripe.net/search/query.html) that gives us this next information:

* inetnum:         **130.206.0.0 - 130.206.255.255**
* netname:         REDIRIS
* descr:           Entidad Publica Empresarial Red.es
* …

- Consultamos en wikipedia las actualizaciones pasadas ([con el siguiente enlace](https://es.wikipedia.org/w/index.php?limit=50&title=Especial%3AContribuciones&contribs=user&target=130.206.0.0%2F16&namespace=&tagfilter=&year=2016&month=-1) .

> Esta búsqueda, requiere que hayamos iniciado sesión en wikipedia. Tambien es necesario permitir búsqueda por rango de Ip's en tus preferencias de wikipedia.

- Calculo de [subnets](https://www.dan.me.uk/ipsubnets?ip=130.206.0.0)


`rediris-networks.json`

### Debugging

If you would like to test without tweeting you can run anon with the `--noop` flag, which w ll cause the tweet to be written to the console
but not actually sent to Twitter.

    ./anon.coffee --noop

If you would like to see all the change activity (URLs for each change) to test that it is actually listening, use the `--verbose` flag:

    ./anon.coffee --verbose

### Alternate Configuration Files

By default anon will look for a `config.json` file in your current working directory. If you would like to specify the location of the configuration file, use the `--config` parameter:

    ./anon.coffee --config test.config

## Develop

There is not much to anon but there is a small test suite, which might come in handy if you want to add functionality.

    npm test

## Which Wikipedias?

This bot uses the [wikichanges](https://github.com/edsu/wikichanges) module to listen to 38 language Wikipedias. 

Check the original project for a list of the [currently supported wikipedias](https://github.com/edsu/anon).

## License:

* [CC0](LICENSE) public domain dedication
