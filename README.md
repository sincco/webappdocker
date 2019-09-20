![WebApps](https://developers.google.com/web/progressive-web-apps/images/pwa-fast_720.png)

#  WebApps Docker for Development

### Apache 2.4 + PHP 7.2 + OPCache + MariaDB + XDebug + NodeJs + npm

### Requirements

**MacOS:**

Install [Docker](https://docs.docker.com/docker-for-mac/install/), [Docker-compose](https://docs.docker.com/compose/install/#install-compose) and [Docker-sync](https://github.com/EugenMayer/docker-sync/wiki/docker-sync-on-OSX).

**Windows:**

Install [Docker](https://docs.docker.com/docker-for-windows/install/), [Docker-compose](https://docs.docker.com/compose/install/#install-compose) and [Docker-sync](https://github.com/EugenMayer/docker-sync/wiki/docker-sync-on-Windows).

**Linux:**

Install [Docker](https://docs.docker.com/engine/installation/linux/docker-ce/ubuntu/) and [Docker-compose](https://docs.docker.com/compose/install/#install-compose).

### How to use

Execute in your terminal, change the *PROJECT* to use the name of your project:

```
curl -s https://raw.githubusercontent.com/sincco/webappdocker/master/init | bash -s PROJECT clone
```

### Panels

When finished, you can access your panels with the ports that the script assigned to each one

**Web server:** http://localhost:port

**PHPMyAdmin:** http://localhost:port

### Features commands

| Commands  | Description  | Options & Examples |
|---|---|---|
| `./init`  | If you didn't use the CURL setup command above, please use this command changing the name of the project.  | `./init PROJECT` |
| `./start`  | If you continuing not using the CURL you can start your container manually  | |
| `./stop`  | Stop your project containers  | |
| `./kill`  | Stops containers and removes containers, networks, volumes, and images created to the specific project  | |
| `./shell`  | Access your container  | `./shell root` | |
| `./grunt-init`  | Prepare to use Grunt  | |
| `./grunt`  | Use Grunt specifically in your theme or completely, it'll do the deploy and the watcher.  | `./grunt luma` |
| `./xdebug`  |  Enable / Disable the XDebug | |
| `./composer`  |  Use Composer commands | `./composer update` |
| `./npm`  |  Use npm commands | `./npm run dev` |

### License

[Iván Miranda](https://ivanmiranda.me) [based on](https://hub.docker.com/r/rafaelcgstz/magento2/) https://hub.docker.com/r/rafaelcgstz/magento2/.
