<h1 align="center">Welcome to Rock Shop 👋</h1>
<p>
  <img src="https://img.shields.io/badge/version-1.0.0-blue.svg?cacheSeconds=2592000" />
</p>

![](/image/logo.png)

## Description

https://drive.google.com/file/d/1SAkY1Qyb5ThbOJXg7R8nlZivb31H49fq/view?usp=sharing

![API_Gateway](https://github.com/vinhyenvodoi98/rock_shop_microservice/blob/master/DocsImages/gateway.png)

## Run

```sh
  docker-compose up
```

## API_Gateway

Set up upstreams , services, routes in ./API_Gateway_service/compose/kong/declarative

If you want to edit the file `kong.yml` while it is running, remember run

```sh
docker-compose exec kong_API_Gateway kong reload
```

For reload Kong

### Upstreams

Targets are the destinations that our Upstream targets are essentially the addresses of the servers that host the services. For each server, we will create a corresponding target

### Services

Service entities, as the name implies, are abstractions of each of your own upstream services. Examples of Services would be a data transformation microservice, a billing API, etc.

### Route

A route is a set of rules for Kong match requests to exactly the API on the services it needs.

## Auth_service

[API contact](https://github.com/vinhyenvodoi98/rock_shop_microservice/blob/master/auth_service/Readme.md)
