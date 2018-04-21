# PHP Docker Setup for learning PHP 

## Installation
1. Make sure you have Docker installed. `brew install docker`, `sudo apt-get install docker`, or download Docker directly from their website.
2. Download and install Docker Compose. It let's us manage Docker easier. 

## Getting setup
1. Open your command line (Bash for Ubuntu for Windows, Terminal, Bash.. which ever you prefer). 
2. `cd` to the directory you want to learn PHP inside. This is usually your Documents folder.
3. `git clone https://github.com/KalobTaulien/PHP-Docker.git learn_php` this will clone this repo onto your computer. (You may need to download `git` for this to work; otherwise you can download the .zip of this repo)
4. `cd learn_php` or open Explorer/Finder and navigate to where your new files (the ones in this repo) are located. 
5. Run `make build` (you may need to install a package to use the Makefile). 
6. Run `make up`
7. Run `make enter`. This will open your new Docker container (think of it as an operating system inside your operating system; to exit the container type `ctrl+d`)
8. Run `service apache2 start` to start Apache inside your Docker container. Apache is the software that reads your PHP.
9. Go to `http://localhost:8000/index.php` and you should the welcome message! 

## Turning it off
To turn off your Docker container, type `make down`. To remove it entirely, type `make clean`. 

## Viewing your containers
To view all your containers, type: `docker container ls -a`. It will list your container name, id, ports and bindings, etc. 

## Got stuck?
If you're using this to learn PHP and you've gotten stuck and you're frustrated, feel free to download XAMPP from https://www.apachefriends.org/download.html -- it will take care of all of this for you. ;) 