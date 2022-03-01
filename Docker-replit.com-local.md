## Levantar la App en local
Comando para levantar un contendor con PHP para hacer más facil testear la aplicación que creamos en (Replit.com)[https://replit.com]

```bash
docker run -it --rm  -d \
-p 8090:80 \
-v $(pwd):/usr/local/apache2/htdocs/ \
--workdir /usr/local/apache2/htdocs/ \
--name ${PWD##*/} \
httpd:2.4

#windows
docker run -it --rm  -d \
-p 8090:80 \
-v ${PWD}:/usr/local/apache2/htdocs/ \
--workdir /usr/local/apache2/htdocs/ \
httpd:2.4
```

##### Plugins a instalar:
Se recomienda instalar los plugins:
- Better Comment
- Trailing Spaces
- Docker
