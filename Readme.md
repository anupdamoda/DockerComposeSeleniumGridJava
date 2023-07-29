# Docker compose file for the Selenium Grid Server

This project contains the docker compose file which when run creates the Selenium hub server.
and made the source code freely available under the [Apache License 2.0](LICENSE.md).

These Docker images come with a handful of tags to simplify its usage, have a look at them in one of
our [releases](https://github.com/SeleniumHQ/docker-selenium/releases/tag/4.10.0-20230607).

To get notifications of new releases, add yourself as a "Releases only" watcher.

These images are published to the Docker Hub registry at [Selenium Docker Hub](https://hub.docker.com/u/selenium).

## Quick start

## Execution modes ## 🤖 Starting up

### Selenium Grid : hub and nodes setup

```bash
docker compose up
```

### Standalone

![Firefox](https://raw.githubusercontent.com/alrra/browser-logos/main/src/firefox/firefox_24x24.png) Firefox
```bash
docker run -d -p 4444:4444 --shm-size="2g" selenium/standalone-firefox:4.10.0-20230607
```

![Chrome](https://raw.githubusercontent.com/alrra/browser-logos/main/src/chrome/chrome_24x24.png) Chrome
```bash
docker run -d -p 4444:4444 --shm-size="2g" selenium/standalone-chrome:4.10.0-20230607
```

![Edge](https://raw.githubusercontent.com/alrra/browser-logos/main/src/edge/edge_24x24.png) Edge
```bash
docker run -d -p 4444:4444 --shm-size="2g" selenium/standalone-edge:4.10.0-20230607
```

_Note: Only one Standalone container can run on port_ `4444` _at the same time._

___

### Hub and Nodes

There are different ways to run the images and create a Grid with a Hub and Nodes, check the following options.


