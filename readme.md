# BPO Project Laravel Homestead Configuration

The official Laravel local development environment.

Official documentation [is located here](http://laravel.com/docs/homestead?version=4.2).

## Included Software as per official [Laravel Homestead] (http://laravel.com/docs/homestead)

* Ubuntu 14.04
* PHP 5.5
* Nginx
* MySQL
* Postgres
* Node (With Bower, Grunt, and Gulp)
* Redis
* Memcached
* Beanstalkd
* Laravel Envoy
* Fabric + HipChat Extension

## Instrucctions
1. Adding The Vagrant Box

Once VirtualBox and Vagrant have been installed, you should add the laravel/homestead box to your Vagrant installation using the following command in your terminal. It will take a few minutes to download the box, depending on your Internet connection speed:

`vagrant box add laravel/homestead`

How to see if the box is available in Vagrant? Execute the following command:

`vagrant box list`

You should see the following description in the box list: laravel/homestead      (virtualbox, 0.1.6) 

2. Clone this repository - 
Once the box has been added to your Vagrant installation, you should clone or download this repository. Consider cloning the repository into a central Homestead directory or in the desire folder where you keep all of your Laravel projects, as the Homestead box will serve as the host to all of your Laravel (and PHP) projects. 

`git clone https://github.com/jamesxv7/homestead.git bpo`
