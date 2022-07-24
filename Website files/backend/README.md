# Project: Dad-Joke-Backend-Service

## Getting Started
---
### Prerequisite
---

This project is containerized. Please have Docker installed.  Instructions are
on the README in the project root.

### Development
---
#### Install
Running this command will install all the dependencies for the backend project.

```bash
npm install
```

#### Start Development Server
Running this command will start the development server.  The endpoint is at port 8000.

```bash
npm start
```

#### Build
Running this command will build a production ready version of the project.

```bash
npm run build
```

#### Lint
Running this command will run ESLint on the backend project.

```bash
npm run lint
```

### Using Dockerfile
___
#### Build the Image
This command has to be ran from within the backend directory.

```bash
docker build --tag dadjokebackend .
```

#### Build the Container
This command will build and run the container in detached mode.  You will be able to hit the container on port 8000.

```bash
docker run -d --name dadjokebackend -p 3000:3000 dadjokebackend
```

#### Removing the Container
This command will kill the running container and remove it.

```bash
docker rm -f dadjokebackend
```
