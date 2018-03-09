# c9-lmp

This repo holds all the script, config files and commands that you might want to
use to set up a LEMP environment using NGINX and PHP-FPM instead the default
Apache2 runner for PHP applications on Cloud9 workspaces.

### Prerequisite

Setup a c9 workspace using the Apache, PHP5 and MySQL template

### Usage

Run any of this commands straightaway on your c9 terminal.

``` bash
curl -L https://raw.githubusercontent.com/GabrielGil/c9-lemp/master/install.sh | bash
```
----
``` bash
wget -O - https://raw.githubusercontent.com/GabrielGil/c9-lemp/master/install.sh | bash
```

After completing this process your environment will also be provisioned with a
simple command to start, stop and restart the whole stack in a brief:

* `lemp start` // Starts NGINX and PHP
* `lemp stop`
* `lemp restart`
* `lemp status`

### Updating

You can re-run this script as many times as you wish, just in case something is updated.


### Considerations

This is a quite simple script. It is just an easy way to configure your environment
to be up and running with NGINX and PHP-FPM.

It does not override the default NGINX site configuration file, so you don't have to
worry about loosing any data in case you had already modified yours.
