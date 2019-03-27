# PHP-CLI

The container after build will contain latest PHP CLI Interpreter
installed on latest Ubuntu.

------------

[Github](https://github.com/ABGEO07/docker4dev/tree/master/PHP-CLI "Github")

[Docker Hub](https://hub.docker.com/r/abgeo/d4d-php-cli "Docker Hub")

------------

### Pull / Build

You can get container from Docker Hub `docker pull abgeo/d4d-php-cli:v0.9`
Or build from Dockerfile `docker build -t d4d-php-cli {path-to-Dockerfile}`.

### Run

After pull or build you must run the container.

If you pull it from hub, you can start container by running `docker run -v {path-to-php-scripts-folder}:/usr/src/scripts -it abgeo/d4d-php-cli:v0.9`
or if you build it manually you can run `docker run -v {path-to-php-scripts-folder}:/usr/src/scripts -it d4d-php-cli` where `d4d-php-cli` is your build name.

After run you can access you'r container bash environment and run php scripts.

#### Volumes
Your container must implement one volume to path `/usr/src/scripts`.
Ex.: `... -v {path-to-php-scripts-folder}:/usr/src/scripts ... `
