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