#This is a Work in progress. 

The main idea is a series of scripts for linux that simulates this alfred extension:

https://github.com/clarkeash/Laravel-Alfred-Extension 

Help is welcome to acomplish this task.

#What Works right now:

###Create new project

    laravel new testproject

This command will:

- Clone a laravel instalation from github to a defined directory and rename it to project_name(change this parameter as you need).
- Create a symlink from you development directory to your local server public directory. 
- Set the correct file permissions to the storage directory inside laravel installation.
- Download and install laravel generators (https://github.com/JeffreyWay/Laravel-Generator)

###Generate new resource
    
    laravel r testproject post 

This command will create:
  - A post.php model
  - A posts.php controller 
  - A post views folder with index.blade.php view.

###Generate assets

    laravel testproject assets main.scss scripts.js

This will create two files:

    public/css/sass/main.scss
    public/js/scripts.js

The default directory paths are:

- CSS => public/css/
- JavaScript => public/js/
- CoffeeScript => public/js/coffee/
- Sass (sass or scss extension) => public/css/sass

#Installation

I'm working to make this process more friendly, for now you need to:

- Download or clone this repo to your home folder
- Rename the downloaded folder to .fsp_laravel
- Run the following command:

    ln -s ~/.fsp_laravel/laravel /usr/local/bin/laravel

# Usage

If you are using unity, simply open de run command interface (Alt+F2) and type any of the available commands.

This should also work with gnome-do, synapse, krunner, and any other program that can run linux commands stored in /usr/local/bin
