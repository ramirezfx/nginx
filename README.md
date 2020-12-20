# nginx

Get the file:

`git clone https://github.com/ramirezfx/nginx.git`

Change the file docker-compose.yml if needed.

Compile/Start the container:

`docker-compose up -d`

Copy the website-directory or file to the docker container:

`docker ps` to get the container-name

Then copy the directory/file to the container:

`WEBSITE=index.html`

`CONTAINERNAME=nginx_nginx_1`

`docker cp $WEBSITE $CONTAINERNAME:/usr/share/nginx/html`
