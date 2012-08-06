# Google Plus status update library

* Readme date: Aug 6 2012
* Contributors: lukapusic, adlerweb
* Author: Luka Pusic <luka@pusic.si>, Florian Knodt <adlerweb@adlerweb.info>
* URI: https://github.com/adlerweb/gplus-bot
*      https://github.com/lukapusic/gplus-bot
*      http://360percents.com/posts/first-google-google-plus-status-update-bot-in-php/

## Description
This library allows you to post status updates to your Google+-Account. It uses username and password by emulating a browser, no API/OAuth required. Based on Luka Pusics GPlus-Bot.

## System requirements
* PHP curl extension

## Instructions
1. include library file into your script 
2. Start new instance: $gp = new gplusBot('yourmail@gmail.com', 'yourpassword');
3. Post message: $gp->update_profile_status($p);

##Notes
This is mainly designed for CLI/single user - if you want to use concurrent connections
please read (and understand!) this script first

## Changelog

#### Nov 11 2011
* added debug parameter, pageid parameter, pc_uagent parameter
* page updating still not implemented

#### Nov 16 2011
* changed the way baseurl is determined, google removed base href

#### Dec 15 2011
* post visibility is not public by default

#### Mar 2 2012
* fixed "&" encoding (thx Pauly)

#### Auf 6 2012
* Changed plain PHP-script to library

## Known issues
* fails if you didn't confirm mobile location terms and conditions
* fails if you have mobile verification enabled

## TODO
* add an option to change post visility
* add posting to pages
* add image upload
* add URL upload

## License
 ----------------------------------------------------------------------------
 "THE BEER-WARE LICENSE" (Revision 42):
 <luka@pusic.si> wrote this file. As long as you retain this notice you
 can do whatever you want with this stuff. If we meet some day, and you think
 this stuff is worth it, you can buy me a beer in return. Luka Pusic
 ----------------------------------------------------------------------------
