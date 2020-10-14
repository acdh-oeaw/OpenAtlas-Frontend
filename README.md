# OpenAtlasDiscovery

# About

OpenAtlasDiscovery is a presentation webapp for [OpenAtlas](https://openatlas.eu) projects.

At the moment we are in the concept phase and this is just a basic start point for further development.

# Licensing

All code unless otherwise noted is licensed under the terms of the MIT License (MIT).
Please refer to the file COPYING in the root directory of this repository.

All documentation and images unless otherwise noted are licensed under the terms of Creative Commons Attribution-ShareAlike 4.0 International License.
To view a copy of this license, visit http://creativecommons.org/licenses/by-sa/4.0/

# Technology

The webapp is built using the [nuxtjs](https://nuxtjs.org/) framework based on [Vuejs](https://vuejs.org/)

# Setup

Whilst the app ultimately runs in the browser and can be served from any webserver developing and deploying it
requires [NodeJS](https://nodejs.org/en/about/releases/) (minimum v10, current LTS is recommended) 

After cloning the repository, install all dependencies with
```bash
$ npm install
```

Furthermore a running OpenAtlas instance with an activated [API Module](https://demo.openatlas.eu/static/manual/tools/api.html) is required.
The instance served needs to be documented in the [Server Object](https://swagger.io/specification/#server-object) of
the OpenAPI specification here:

```
\assets\swagger.json
``` 

## For Development

```
# serve with hot reload at localhost:3000
$ npm run dev
```

## For Deployment

```
# generate the project files to /dist
$ npm run export
```

The resulting files in the /dist folder can be served from any web server or be exposed through nuxt using

```
npm run server
```

For detailed explanation on how things work, check out [Nuxt.js docs](https://nuxtjs.org).
