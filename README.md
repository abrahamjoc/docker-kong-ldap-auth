# docker-kong-ldap-auth
Docker Kong and LDAP Server at one

# How to use this template

This Docker Compose template provisions a Kong container with a Postgres database, plus a nginx load-balancer. After running the template, the `nginx-lb` load-balancer will be the entrypoint to Kong.

To run this template execute:

```shell
$ docker-compose up
```

To scale Kong (ie, to three instances) execute:

```shell
$ docker-compose scale kong=3
```

In case of error with COMPOSE_HTTP_TIMEOUT: run on this way:

```shell
$ COMPOSE_HTTP_TIMEOUT=3600 docker-compose up
```

## Information

https://docs.konghq.com/hub/kong-inc/ldap-auth/

https://github.com/sharmalab/bindaas/wiki/Configure-the-ldap-auth-plugin-for-a-Service-with-Kong

## Other repos
https://github.com/abrahamjoc/docker-compose-kong-konga

https://github.com/abrahamjoc/docker-compose-ldap-server
