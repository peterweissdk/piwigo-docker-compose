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


**Free Software... But of Course!**

Copyright [2023] [PeterWeissDK]

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.

###### _I used [Dillinger](https://dillinger.io) to create this file_

[//]: # (misc. -comments)
