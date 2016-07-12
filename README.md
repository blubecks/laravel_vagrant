#Vagrant

I've find in Vagrant one of the best dev team's tool.

This repository is in fact an extract of my vagrant_test repository (https://github.com/andreafspeziale/vagrant_test/tree/laravel-development).

I'm actually using this vagrant to run my learning_laravel_5 sample app
(https://github.com/andreafspeziale/learning_laravel_5).

#Options

    - vars:
        document_root: PATH_OF_APPLICATION (es: /vagrant/NAME_OF_THE_PROJECT/public)
        db: TYPE_DB

#Installing

Packages that will be installed

##Commons

    - git
    - vim
    - grunt
    - bower
    - curl
    - composer

##Database

Set in the playbook your db preference

    - mongodb

or

    - mysql

##Webserver

    - apache2
    - node
    - php
    - phpmyadmin

#Laravel

Now you should be ready to start a new laravel project from scratch.

Once you runned vagrant up:

    - $ vagrant ssh
    - $ cd /vagrant
    - composer create-project --prefer-dist laravel/laravel NAME_OF_THE_PROJECT

Go to your browser and type localhost:8080, you should see laravel welcome page
