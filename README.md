# Goal:

same development environment as in prod:

traefik ingress controller -> SSL 443
send http/tcp trafic to dotnet core app -> 80

setup a local revers proxy on 443
and rout to the docker running on localhost port xx.

docker run -d -p 8080:80 -v /D:/_dev/tomsolem/localproxy/my.conf:/etc/nginx/conf.d/default.conf nginx

# problems with 2 pods using openIdConnect

https://www.kevindockx.com/solving-correlation-failed-state-property-not-found-errors-openid-connect-middleware-asp-net-core/

