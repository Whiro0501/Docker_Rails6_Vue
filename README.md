# README

## Purpose

This is a start-up kit for a  Docker of Rails and Vue Applications

## Instruction
1. Git clone this repository
2. Run "docker-compose build" to build Docker image.
3. Run "docker-compose run web yarn install --check-files" get necessary node modules.
4. Run "docker-compose run web rake db:create" to crteate Postgresdb.
5. Run "docker-compose up" to start the rails application
6. Run "docker-compose exec web ./bin/webpack-dev-server" 
7. Access to "http://localhost:3000/" on Web browser.

## Available Scripts

In the project directory, you can run:

```
docker-compose build

docker-compose run web yarn install --check-files

docker-compose run web rake db:create

docker-compose up

docker-compose exec web ./bin/webpack-dev-server

```

Connet Rails to Vue
```
<%= javascript_pack_tag 'hello_vue' %>
<%= stylesheet_pack_tag 'hello_vue' %>
```

Runs the app in the development mode.

Open http://localhost:3000 to view it in the browser.
