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
###Prerequisites

* [Virtual Box](https://www.virtualbox.org/)
* [Vagrant](https://www.vagrantup.com/)
* [Git](http://git-scm.com/)

###Adding The Vagrant Box

Once **VirtualBox** and **Vagrant** have been installed, you should add the **laravel/homestead** box to your Vagrant installation using the following command in your terminal. It will take a few minutes to download the box, depending on your Internet connection speed:

`vagrant box add laravel/homestead`

How to see if the box is available in Vagrant? Execute the following command:

`vagrant box list`

You should see the following description in the box list: laravel/homestead      (virtualbox, 0.1.6) 

###Clone this repository 

Once the box has been added to your Vagrant installation, you should clone or download this repository. Consider cloning the repository into a central Homestead directory or in the desire folder where you keep all of your Laravel projects, as the Homestead box will serve as the host to all of your Laravel (and PHP) projects. 

`git clone https://github.com/jamesxv7/homestead.git bpo`

###Launch The Vagrant Box

Once you have edited the Homestead.yaml to your liking (if necesary), run the vagrant up command from the **bpo** directory in your terminal. Vagrant will boot the virtual machine, and configure your shared folders and Nginx sites automatically!

`vagrant up`

###SSH Homestead Virtual Machine to Install Laravel

First execute the following command in the terminal window.

`vagrant ssh`

If everything goes correct proceed to install Laravel.

`composer create-project laravel/laravel --prefer-dist`
