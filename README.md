# privateAndNotPrivatePackages

- run composer install
- check in vendor folder, private packages have installed


// code for packages


    {
        "repositories": [
            {
                "type": "vcs",
                "url": "https://github.com/ultimecreation/MittasciencePrivate"
            }
        ],
        
        "autoload": {
            "psr-4": {
                "Moi\\Composer03\\": "src/"
            }
        },
        "require": {
            "mittascience/test-notprivate": "dev-master",
            "mittascience/private": "dev-master"
        }
    }


// code to create a project

- add the code below to your project/framework (the name has to be "vendor/package" )

    {
        "name": "ultimecreation/php-mvc-for-example",
        "description": "A basic mvc implementation for beginners",
        "type": "project",
        "license": "MIT",
        "require": {}
    }

- list your project/framework on packagist
- then you can use this kind of command line LIKE BELOW
    => composer create-project ultimecreation/php-mvc:dev-master
    => composer create-project ultimecreation/php-mvc:1.0.0 OR WHATEVER tag that you will have created