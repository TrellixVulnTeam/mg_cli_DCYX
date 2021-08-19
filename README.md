# Mg_cli
With this CLI tool you can make modules dynamically for the Magento frame-work faster better cleaner 

Ditch the online module makers!
Have one built in in your cli

---
# Table of Contents
1. [Install](#install)
2. [How to Use](#quickstart)
4. [Commands](#commands)
5. [ToDo](#todo)
6. [features ideas](#features--ideas)

## Install

 1. `git clone https://github.com/IasonArgyrakis/mg_cli.git`
 2. `cd mg_cli` 
 3. `cd npm install` to download all the required libs
 3. `npm install -g . ` to install the current dir as a library 
 
 One Line Install: `git clone https://github.com/IasonArgyrakis/mg_cli.git && cd mg_cli && npm install -g . `
 


## Quickstart

   `mg g`
--

`--register` to make `registration.php` & `composer.json`

`--b` for Block

`--ctr` for Controler

`--mdl` for Model

## Guide


`mg g --b myblockname` 

To make a `Block` folder with a `myblockname.php` inside

---
`mg g --b myotherblockname --e`

To make a `Block` folder with a `myotherblockname.php` that extends `\Magento\Backend\Block\Widget\Grid\Container`

---

`mg g --b myotherblockname --e yourStringHere`

To make a `Block` folder with a `myotherblockname.php` that extends `yourStringHere` 
NOTE: the terminal does not recognise backslashes !

---

`mg g --ctr myotherblockname `

To make a `Controler` folder with a `myotherblockname.php`  
NOTE: the terminal does not recognise backslashes !

---

`mg g --mdl myotherblockname `

To make a `Model` folder with a `myotherblockname.php`  
NOTE: the terminal does not recognise backslashes !


---
## Assists for Dev

https://developer.okta.com/blog/2019/06/18/command-line-app-with-nodejs

https://medium.com/@pongsatt/how-to-build-your-own-project-templates-using-node-cli-c976d3109129

https://magefan.com/blog/create-block-template-layout-in-magento-2

node_modules/.bin/semver


---
## Commands

Modes : What the command does 

Case : Where it does it ( will the consumer ever see it ) 

Parameters :  Is it a custom implementation of smth ? 

`--Block` `--Helper` `--Controler` `--etc` `--Model` `--Observer` `--view`

Atributes : How it does it ( example: Do you want `js` | `css` )

Directives : placeholder

---

## ToDo 

[x]  Make Hello Wolrd  

[x]  Parse Complex filenames

[x]  make or copy Complex filenames to pwd dir

- [x]  Make ProtoTemplates

-[ ]  Make ProtoTempaltes for Vendor_Overides Note: fallbacks 

Milestone One -[ ] 

-[ ]  Make CLI guide

Milestone One_point_TwentyFive -[ ] 

 -[ ]  Intergrate ProtoTempaltes variables

Milestone One_point_five -[ ] 

-[ ]  Intergrate ProtoTempaltes variables for Vendor_Overides

-[ ]  XML Directives (add the mg_generated_module to a view  index | static-page | product-category 

-[ ]   add the mg_generated_module

-[ ]   integration with directives for subfolders of each class created. Must be multiple directives and subfolders as well

-[ ]   camel case validation for class names passed as directives


---

##  Features | Ideas 

Stuff to make using the tool 

nonoce-js (make a js pool of scripts) for head | body | blocks etc using observers 

ez-ass-pie dynamiclaly build and add layout `xml` `phtml` for pages such as Index | category | product | custom-feature
* custom-feature placeholder for custom ui stuff
   example  [Azera](https://azera.smart-digital.gr/?templatehints=magento)
   `/var/www/vhosts/smart-digital.gr/azera.smart-digital.gr/app/design/frontend/DigitalUp/diogenes/DigitalUp_Diogenes/templates/html/homepage/sections/services.phtml`




