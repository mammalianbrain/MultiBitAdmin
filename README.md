# MultiBit Admin

This module is the administration tool and is built with the following:

* Java
* MBM - Providing the heavy lifting for back end merchant operations
* Dropwizard - Serves HTML and JavaScript, intermediates with the MBM platform
* Bootstrap - A JavaScript framework providing a simple CSS scheme
* jQuery - A JavaScript framework providing a variety of utilities

It is intended as the main user interface to make administrative changes to the platform. 
This includes reviewing accounts, manually raising invoices, purchase orders and so on.
This is the module that the staff working for your organisation would use in their day to
day operations.

## Notation

<project root> - The root directory of the project as checked out through git

All commands will work on *nix without modification, use \ instead of / for Windows.

## Getting started

First you must build the MBM project using Maven (see [MultiBitMerchant](https://github.com/gary-rowe/MultiBitMerchant) repo)

    cd <MBM project root>
    mvn clean install

You will need to have MBM running in a separate process. From the console you can do the following

    cd <MBM project root>/mbm
    java -jar target/mbm-develop-SNAPSHOT.jar server mbm.yml

Next, you will need to build this project

    cd <Admin project root>
    mvn clean install

Finally, you can start it with

    cd <Admin project root>
    java -jar target/admin-develop-SNAPSHOT.jar server admin.yml

## Where does the ASCII art come from?

The ASCII art for the startup banner was created using the online tool available at
[Webestools][http://www.webestools.com/ascii-text-generator-ascii-art-code-online-txt2ascii-text2ascii-maker-free-text-to-ascii-converter.html]
with a font of Tiza