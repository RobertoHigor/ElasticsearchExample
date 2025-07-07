# About this repository

This repository contains an example project that uses elasticsearch.
The project consists on a frontend made with vue 3, and a api built with .net 9 to interact with elasticsearch.

## Docker compose

`docker compose up --build`

You can access the frontend project through `http://localhost:80` and the backend through `http://localhost:8081/swagger`

## Developer build

Api port 8080
`watch run --project .\Api\api.csproj`

Frontned port 80
`npm install vite`
`npm run dev`

## Running the projects individually

### Running frontend

Building the image with the image named "frontend"`

`docker build -t frontend .\frontend\`

Running the project
`docker run -it -p 8080:80 frontend`

### Running backend

Building the image named "backend"

`docker build -t backend .\backend\`

Running the project with docker

`docker run -it -p 8081:5282 backend`

If you run without docker, you an acess it through the url `http://localhost:8080`

