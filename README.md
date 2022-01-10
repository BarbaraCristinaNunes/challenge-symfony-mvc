# challenge-symfony-mvc

## Learning objectives
* Install Symfony
* Learn about the lifecycle of software
* Learn to use the MVC layer of Symfony
* Learn to use the routing component
* Learn the basics of twig

----
## Steps

### 1. Isntalling Composer
I have a local folder called GitHub where I work with all progects and keep my repositories.

There I opened an cmd terminal and typed the following code:

>php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"

>php -r "if (hash_file('sha384', 'composer-setup.php') === '906a84df04cea2aa72f40b5f787e49f22d4c2f19492ac310e8cba5b96ac8b64115ac402c8cd292b8a03482574915d1a8') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"

>php composer-setup.php

>php -r "unlink('composer-setup.php');"

From https://getcomposer.org/download/

Then using PowerShell terminal I installed [GoFish](https://gofi.sh/#install) package manager using the following code:

>Set-ExecutionPolicy Bypass -Scope Process -Force
iex ((New-Object System.Net.WebClient).DownloadString('https://raw.githubusercontent.com/fishworks/gofish/main/scripts/install.ps1'))

Then:
>gofish init

Then: 
>gofish install gofish

Then:
>gofish upgrade gofish

I installed [Symfony](https://symfony.com/download) using the following code:

> gofish rig add https://github.com/symfony-cli/fish-food

>gofish install github.com/symfony-cli/fish-food/symfony-cli

### Create Symfony project

> symfony new MY_PROJECT_NAME