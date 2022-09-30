# README

This project implement rails development with docker and docker compose.

## Usage

1. clone project
1. edit .env file
   * set WEB_IMAGE enviroment variable
   * set PORT enviroment variable to prevent conflict
1. run
   * docker-compose run web rails new . -d postgresql -f
   * docker-compose build
   * docker-compose up
1. run in other shell
   * docker-compose run web rails db:prepare

## Edit application

Remember to run *docker-compose build* if change Gemfile and/or Gemfile.lock
