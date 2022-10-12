# Piwigo
## _Docker Compose file for Piwigo photo management_


This Docker compose file include the base images from linuxserver/mariadb and linuxserver/piwigo
This setup is testet on a Raspberry Pi 3 running Ubuntu 22.04 headless server.

### _My setup:_
- Piwigo
- MariaDB
- Ubuntu 22.04
- Raspberry Pi 3 Model B Plus Rev 1.3

## Installation

Piwigo-docker-compose requires [docker compose](https://docs.docker.com/compose/) version 3 to run.

Install Docker, download the  docker-compose.yml and spin up the container

```sh
git clone https://github.com/peterweissdk/piwigo-docker-compose
docker compose up -d
```

Check that everything is up and running

```sh
docker ps
```

Stop running container

```sh
docker compose down
```
## Note!!!
If you are running a HTTP Piwigo server behind af HTTPS reverse proxy server, and the proxy server handles the ssl certificates, you might not be able to see your photos in the official mobile app. Only empty thumpnails and empty photos will appear. Try to incorporate *http-request set-header X-Forwarded-Proto https if { ssl_fc }* in your reverse proxy setup.

**Want to contribute? Go ahead...!**

This is a standard docker compose file, with no magic tricks.
Make a change in your docker-compose.yml file and instantaneously see your updates!

## License

MIT

**Free Software... But of Course!**

Copyright [2022] [PeterWeissDK]

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

###### _I used [Dillinger](https://dillinger.io) to create this file_

[//]: # (misc. -comments)
