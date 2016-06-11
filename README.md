# docker-grav
A docker image from ALPINE Linux with NGINX, PHP-FPM through unix socket and preinstalled GRAV.


Running a new **Grav** site is a simple affair with [Docker](https://docker.com).  Simply follow these simple steps:

1. Install [Docker](https://docs.docker.com/mac/step_one/).
2. Launch docker terminal and start run a container in the background, mapping port 80 of your vm/host to the port 80 of grav container:

        $docker run -d -p 80:80 --name grav oleglab/grav:latest

3. Open your new site on port 80 and follow the Grav's instructions...
4. To install [admin plugin](https://getgrav.org/downloads/plugins) execute the following command:

       $docker exec grav sh -c 'cd /www && php bin/gpm install admin' 

5. Open / - home page, or /admin - for site administration. Enjoy!!!
