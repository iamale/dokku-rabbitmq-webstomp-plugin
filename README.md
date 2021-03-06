RabbitMQ plugin for Dokku
=========================

This fork [enables the Web-Stomp plugin for RabbitMQ](https://github.com/iamale/dokku-rabbitmq-webstomp-dockerfiles/commit/4df2cb16cc76ebc96212b605552bec905be6054a).

---

Project: https://github.com/progrium/dokku

Requirements
------------
* Docker version `0.7.2` or higher
* Dokku version `0.2.1` or higher

Instalation
-----------
```
cd /var/lib/dokku/plugins
git clone https://github.com/jlachowski/dokku-rabbitmq-plugin.git rabbitmq
dokku plugins-install
```

Commands
--------
```
$ dokku help
    rabbitmq:create <app>                         Create a RabbitMQ container for <app>
    rabbitmq:clone <app> <trg>                    Clone RabbitMQ container of <app> for <trg>
    rabbitmq:rebuild <app>                        Rebuild RabbitMQ container of <app> (keep persistend data)
    rabbitmq:delete <app>                         Delete specified RabbitMQ container for <app>
    rabbitmq:info <app>                           Display <app> RabbitMQ container informations
    rabbitmq:link <app> <rabbit>                  Link an app to a RabbitMQ container
    rabbitmq:list                                 Display list of RabbitMQ containers
    rabbitmq:logs <app>                           Display last logs from <app> RabbitMQ container
```

TODO:
-----
- fix volumin delete (fix access rights)
- improve creation time
- add peristent logs

Thanks
------
This is partially based on the dokku redis plugin: https://github.com/luxifer/dokku-redis-plugin
