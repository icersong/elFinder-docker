# Docker Container for elFinder

This container contains https://github.com/Studio-42/elFinder

# Usage

The container listens on port 80 for connections and serves the '/data' directory

    $ sudo docker run -it --rm -p 8080:80 -v $(`pwd)`:/data icersong/elfinder

The default configuration can be overridden by replacing the file /config/connector.php

    $ sudo docker run -it --rm -p 8080:80 -v `$(pwd`):/data -v connector.php:/config/connector.php icersong/elfinder
