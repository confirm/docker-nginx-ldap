About
=====

The nginx-ldap Docker image provides a container, that contains a [nginx server](http://nginx.org/) with LDAP support.

This [nginx-auth-ldap](https://github.com/kvspb/nginx-auth-ldap) module is used for LDAP support.


Usage
=====

The docker image can be used like the [official nginx docker image](https://hub.docker.com/r/library/nginx/).
But you have to overwrite the configuration file like to configure the LDAP authentication.

```
$ docker run --name some-nginx -v /some/nginx.conf:/etc/nginx/nginx.conf:ro -d nginx
```

LDAP configuration
------------------

The documentation for the LDAP authentication and an example is [here](https://github.com/kvspb/nginx-auth-ldap/blob/master/README.md#example-configuration) available.


Nginx Configuration
===================

Here are some further links for more configuration hints.

* [official nginx documentation](http://nginx.org/en/docs/configure.html)
* [nginx tuning documentation](https://www.nginx.com/blog/tuning-nginx)
* [ldap module documentation](https://github.com/kvspb/nginx-auth-ldap/blob/master/README.md)


Registry
========

This image is an automated build on the [official Docker Hub](https://hub.docker.com/r/confirm/nginx-ldap).
