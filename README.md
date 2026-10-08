# docker-website-demo

A simple web page packed into a Docker container and served by nginx. Built to learn the basics of Docker.

## What's inside
- `index.html`: a simple web page
- `Dockerfile`: the recipe that starts from a small nginx image, copies the page into it and opens port 80

## How to run
You need Docker Desktop running. In a terminal, from this folder:

    docker build -t my-website .
    docker run -d -p 8080:80 --name my-website-container my-website

Then open `localhost:8080` in your browser.

## To stop and remove it
    docker stop my-website-container
    docker rm my-website-container

## Result
![Website running in Docker](Docker_webpage%202026-10-08%20073754.png)

## Tools
Docker, nginx, HTML
