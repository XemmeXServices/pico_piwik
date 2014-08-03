Pico Piwik
===============

Adds automatically the Piwik tracking script to the end of body section of each page of the site.

## Installation

Place `pico_piwik.php` file into the `plugins` directory.

## Configuration

Inside the `config.php` file:

````
/* PIWIK */
/* Piwik Hostname and Piwik install folder */
// For example : www.example.com or example.com
// If Piwik is install on the same domain as your Pico Site,
// you can let that empty or remove it from config.php
$config['piwik']['domain'] = '';
// If empty or not present, we take "piwik" as default value
$config['piwik']['folder'] = '';
/* Website ID */
//If empty or not present, 1 is the default value
$config['piwik']['id'] = 1;
/* Tracking options */
/* Settings --> Tracking code */
// Track visitors across all subdomains of SITE NAME
$config['piwik']['subdom'] = false; /* true or false */
// Prepend the site domain to the page title when tracking
$config['piwik']['prepend'] = false; /* true or false */
// In the "Outlinks" report, hide clicks to known alias URLs of SITE NAME
$config['piwik']['outlinks'] = false; /* true or false */
// Advanced : Enable client side DoNotTrack detection
$config['piwik']['DNT'] = true; /* true or false */
````

## TODO

- adding support for custom variables ?