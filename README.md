# LWT Docker

A quick local setup of [Learning With Texts][1] using [Docker][2]
and [Docker Compose][3].

## Usage

First you need to have [Docker][2] installed and set up correctly.
This may require creating a VM with [docker-machine][4] - [Kitematic][5] is
a tool which does this automatically.

When docker is set up (output of `docker ps` doesn't complain about connection
issues), you need to clone or download this repo and run:

```sh
docker-compose up -d
```

LWT should be running now, available at the IP address of your docker host
and port 7070.

Feel free to change the timezone in [config/php.ini](config/php.ini) (you'll
need to restart lwt-app docker container to make it work).

[1]: http://lwt.sf.net/
[2]: https://www.docker.com/
[3]: https://docs.docker.com/compose/overview/
[4]: https://docs.docker.com/machine/overview/
[5]: https://kitematic.com/
