# CentOS Application Lite Edition Docker (Application-Lite Container)
[![Build Status](https://travis-ci.org/zeroc0d3lab/centos-application-lite.svg?branch=master)](https://travis-ci.org/zeroc0d3lab/centos-application-lite) [![](https://images.microbadger.com/badges/image/zeroc0d3lab/centos-application-lite:latest.svg)](https://microbadger.com/images/zeroc0d3lab/centos-application-lite:latest "Layers") [![](https://images.microbadger.com/badges/version/zeroc0d3lab/centos-application-lite:latest.svg)](https://microbadger.com/images/zeroc0d3lab/centos-application-lite:latest "Version") [![GitHub issues](https://img.shields.io/github/issues/zeroc0d3lab/centos-application-lite.svg)](https://github.com/zeroc0d3lab/centos-application-lite/issues) [![GitHub forks](https://img.shields.io/github/forks/zeroc0d3lab/centos-application-lite.svg)](https://github.com/zeroc0d3lab/centos-application-lite/network) [![GitHub stars](https://img.shields.io/github/stars/zeroc0d3lab/centos-application-lite.svg)](https://github.com/zeroc0d3lab/centos-application-lite/stargazers) [![GitHub license](https://img.shields.io/badge/license-GPLv2-blue.svg)](https://raw.githubusercontent.com/zeroc0d3lab/centos-application-lite/master/LICENSE.GPL)

This docker image includes:

## Features:
* bash (+ themes)
* oh-my-zsh (+ themes)
* tmux (+ themes)

## Configuration:
* Generate ssh key for your access
  - ssh-keygen -t rsa
* Add your id_rsa.pub to environment (.env) file
* Add your id_rsa.pub to SSH_AUTHORIZED_KEYS in Dockerfile
* Rebuild your docker container
  ```
  docker-compose build && docker-compose up --force-recreate
  ```
* Check your IP Address container
  - `docker ps`
  - `docker inspect [name_container]` (eg: application_1)
* Access ssh
  - `ssh docker@[ip_address_container]`
  - superuser access (root)
    `sudo su` (password: docker)

## License
GNU General Public License v2
