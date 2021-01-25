# Progressive Web App Starter - Javascript

Starter template for a progressive web app with html, css and javascript.

This repo provides a [devcontainer.json](https://code.visualstudio.com/docs/remote/devcontainerjson-reference) to run with vscode [Remote - Containers](https://code.visualstudio.com/docs/remote/containers).

``` text
Remote-Containers:  Clone Repository in Container Volume...
```

[What are Progressive Web Apps?](https://web.dev/what-are-pwas/) and [Introduction to progressive web apps](https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps/Introduction) have descriptions of what a PWA is all about.

## Installable
Installed Progressive Web Apps feel like part of the device they're installed on.

The application must meet some criteria to be accepted as installable by the browser. See the [Chrome PWA Install Criteria](https://web.dev/install-criteria/#criteria)

### Served over https
The application must be served over https to be installable. For local development(localhost) this is relaxed.

### Application Manifest
The [application manifest must exist](https://web.dev/add-manifest/), i.e. linked in the html header of all pages and include specific properties:
  * short_name or name
  * icons
  * start_url
  * display ( fullscreen | standalone | minimal-ui )
  * prefer_related_applications not present or false

### Service Worker
The application must register a service worker with a functional fetch header. As of mid-2021 supposedly the service worker also must handle requests in offline mode


## Reliable
A reliable Progressive Web App feels fast and dependable regardless of the network.

### Offline Capability

## Capable
A Progressive Web App leverages modern web features to provide native-like capabilities.

### Push Messages


## Starter Template


### VSCode Remote Container

This repo is configured as remote container for vscode with a devcontainer.json. You can clone and run it in VSCode with the [Remote-Containers extension](https://code.visualstudio.com/docs/remote/containers).

``` text
Remote-Containers:  Clone Repository in Container Volume...
```

It uses the mcr javascript-node:14 image and post create adds live-server. The configuration file for this is [.devcontainer.json](https://code.visualstudio.com/docs/remote/devcontainerjson-reference)

In the remote container the website can be launched with

``` sh
live-server
```

and with all default settings, vscode should open port 8080 on localhost connected to the live-server in the container.

### Glitch

Just start a new project and clone it from this repository.
