# Intro on Docker

Brief introduction on Docker

To run using Dockerfile: 

    docker build -t web .
    docker run -it --rm --name my-app -p 80:80 web

Using docker-compose:

    docker-compose up -d

Without a Dockerfile:

    docker run --name my-app -v $(pwd)/src:/usr/share/nginx/html -d hhcordero/docker-intro

Read-only mount:

    docker run --name my-app -v $(pwd)/src:/usr/share/nginx/html:ro -d hhcordero/docker-intro
