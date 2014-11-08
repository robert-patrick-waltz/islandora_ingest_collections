# Islandora CONTENTdm Collection Migrator

A utility module for exporting collection configuration data from a CONTENTdm instance and then creating Islandora collections using this data. This module will only be of use to sites that are migrating from CONTENTdm to Islandora.

## Introduction

This module has two main parts: 1) a command-line PHP script that harvests configuration data for collections on a CONTENTdm server and 2) a drush script for creating collections in an Islandora instance using that data. The PHP script outputs the collection data into a tab-separated file so it can be modified prior to being used by the drush script.

Detailed instructions for running the PHP script are provided within the script itself, but in a nutshell, oyou configure a few variables and then run the script. If you have access to your CONTENTdm server's shell and run the script there, the resulting data will contain the title and description for each CONTENTdm collection, plus the collection's thumbnail image. If you don't have access to your CONTENTdm server's shell (e.g., your CONTENTdm is hosted by OCLC), you can run the script from any computer that has PHP installed, but the output will only contain the collection titles.

Once you have the output from the script, you can run the drush command on your Islandora server to create the collections identified in the output.


## Requirements

This module requires the following modules/libraries:

* [Islandora](https://github.com/islandora/islandora)

## Configuration

## Current maintainer:

* [Mark Jordan](https://github.com/mjordan)

## License

[GPLv3](http://www.gnu.org/licenses/gpl-3.0.txt)
