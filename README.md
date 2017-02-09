# Readme of magento-template-me-basic

## Description

Provides basic template directories for Magento themes.

## Installation via composer

Add repository to composer.json

    "repositories": {
        ...
        "meetsecommerce/magento-template-basic": {
          "type": "git",
          "url": "git@bitbucket.org:meetsecommerce/magento-template-me-basic.git"
        },
        ...
    },
    
Add require to composer.json

    "require": {
        ...
        "meetsecommerce/magento-template-basic": "dev-master",
        ...
    },
    
## Adapation

This repository provides a basic structure only and cannot be used out of the box. 

To use it in your project, check out the repository and do the changes you need to do. 

Lets make an example. Your template name will be "supernice" so we need to adapt the follwing parts:

    # Rename directory
    src/app/design/frontend/default/basic   -> src/app/design/frontend/default/supernice
    skin/frontend/default/basic             -> skin/frontend/default/supernice
    
    # Change modman paths
    
    src/app/design/frontend/default/basic/*             app/design/frontend/default/basic/
    src/skin/frontend/default/basic/*                   skin/frontend/default/basic/
    
    # to 
    
    src/app/design/frontend/default/supernice/*         app/design/frontend/default/supernice/
    src/skin/frontend/default/supernice/*               skin/frontend/default/supernice/
    
Don't forget to adapt your composer.json :)
        

 
