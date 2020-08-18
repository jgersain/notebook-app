# Rails App

Diseñado para hacer comprensión conceptual, o sea, no preocuparse tanto por las tecnologías que estan por debajo y de aprenderlas, sino de utilizar interfaces más humanas, abstracciones que permitan llegar aun puto especifico de una forma más rápida

- Aprendizaje JIT (Just in Time), no hay que aprender todo para 
comenzar a desarrollar

- Principio DRY (Convención sobre configuración)

- Diseñado para construir rápido y automátizar

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

### Install Bundler and enable secure HTTP requests

- `gem install bundler`

- `bundle config github.https true`

### Create a new project

- `gem install rails`

- `rails new mi_app`
