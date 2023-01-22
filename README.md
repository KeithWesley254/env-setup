# env-setup

# Frontend ubuntu 20.04
sudo passwd ubuntu

sudo apt install curl git

curl https://raw.githubusercontent.com/creationix/nvm/master/install.sh | bash

<!-- (restart terminal after install) -->
nvm install node 

<!-- (host a static website)  -->
npm install -g serve

screen serve -s build -p 4000

<!-- (eg. screen serve -s build -p 4000) - targets build folder and starts it on another screen -->

# Backend ubuntu 20.04

sudo passwd ubuntu

sudo apt install curl git

gpg --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3 7D2BAF1CF37B13E2069D6956105BD0E739499BDB

\curl -sSL https://get.rvm.io | bash -s stable

<!-- (restart terminal) -->

rvm install 2.7.4 --default

gem update --system

gem install bundler

sudo apt install postgresql postgresql-contrib libpq-dev

<!-- (set postgres passwd) -->
sudo -u postgres createuser -s ubuntu -P

# Git & Github

ssh-keygen

cat ~/.ssh/id_rsa.pub

<!-- copy the key -->