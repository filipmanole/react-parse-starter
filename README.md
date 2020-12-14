<br />
<p align="center">
  <h1 align="center">React and Parse Server Starter</h1>
</p>

## About The Project

This repository contains a simple project with the files needed to start an application user react and parse server.

## Docker images used

- [**mongo**](https://hub.docker.com/_/mongo)
- [**parseplatform/parse-server**](https://hub.docker.com/r/parseplatform/parse-server)
- [**parseplatform/parse-dashboard**](https://hub.docker.com/r/parseplatform/parse-dashboard)
- [**alpine**](https://hub.docker.com/_/alpine)

## Prerequisites

Make sure you have docker and docker-compose installed. If not, follow [this page](https://docs.docker.com/get-docker/)

Clone this repository:

```sh
git clone https://github.com/filipmanole/react-parse-starter
```

## Usage

To start using the project prepare the .env file. You can start from the existing .env.sample:

```sh
cp .env.sample .env
vim .env # edit the file; set the variables properly
```

Use the following command to create a react application inside de frontend directory:

```sh
npx create-react-app frontend/react-app
```

After the you set the variables in .env file, start the reverse-proxy:

```sh
docker-compose up
```

## Default links

After the docker compose was completed successfully, you should be able to access the following links (using default ports):

- [http://localhost:3000/]() - react application
- [http://localhost:4040/]() - parse dashboard
- [http://localhost:1337/playground]() - playground

## Note

The frontend container is configured to use React. It can be modified to use the desired framework.
