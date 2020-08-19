# Notebook App

Aplicación web que maneja tareas como si fuera una libreta

## About the technology

Rails es un framework de desarrollo web diseñado para hacer comprensión conceptual, o sea, no preocuparse tanto por las tecnologías que estan por debajo y de aprenderlas, sino de utilizar interfaces más humanas, abstracciones que permitan llegar aun punto especifico de una forma más rápida.

- Aprendizaje JIT (Just in Time), no hay que aprender todo para 
comenzar a desarrollar

- Principio DRY (Convención sobre configuración)

- Diseñado para construir rápido y automátizar

## Technologies

- Ruby | Ruby on Rails

- Hamlit | SimpleForm

- Bootstrap CSS | JQuery | PopperJS | Roboto FontFace

- Docker | PostgresSQL | Rbenv

## Install Ruby on Ubuntu 20.04 LTS

---

### install necessary libraries

- `sudo apt-get update`

- `sudo apt install build-essential curl wget openssl libssl-dev libreadline-dev dirmngr zlib1g-dev libmagickwand-dev imagemagick-6.q16 libffi-dev libpq-dev cmake libwebp-dev`

### Manage versions with RBENV

- `curl -fsSL https://github.com/rbenv/rbenv-installer/raw/master/bin/rbenv-installer | bash`

- `echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc`

- `echo 'eval "$(rbenv init -)"' >> .bashrc`

- `source ~/.bashrc`

### Install Ruby and set it as default

- `rbenv install 2.7.1`

- `rbenv global 2.7.1`

### Docker and PostgreSQL

- `docker run --name postgres-name -p 127.0.0.1:5432:5432 -e POSTGRES_PASSWORD=developer -e POSTGRES_USER=pgdev -d postgres:latest`

### Install Bundler and enable secure HTTP requests

- `gem install bundler`

- `bundle config github.https true`

## Addictional

- [Template engine Hamlit](https://github.com/k0kubun/hamlit)

- [Simple form](https://github.com/heartcombo/simple_form)

- Document models with annotate: Add `gem 'annotate'` to Gemfile | Run `annotate --models --exclude fixtures`

- Config simple_form with bootstrap `rails g simple_form:install --bootstrap`

- Manage locales `gem install i18n-tasks`

- Debugging: Add `gem 'pry'` and `gem 'pry-doc'` inside Gemfile (developement and test)


## Run project

- `bundler install & yarn`

- `rails s`
