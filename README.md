pl6anet.org
===========

Install instructions and config for pl6anet.org

On a recentish perl install
https://metacpan.org/pod/distribution/Perlanet/bin/perlanet

Select a local data directory and copy all related files in place, eg.
/home/steve/perlanet

Select a target 'webroot' directory on your server and copy
200px-Camelia.svg.png and style.css in place.  The latter file was borrowed
from perl6.org itself :-)

An example webroot on FreeBSD would be /usr/local/www/apache22/data

The config file is perlanetrc and should be modified to refer to your local
data directory and webroot.

Install crontab job template for a user with write permission to the target
webroot

$ crontab < crontab-l

Modify all paths in that cron line to local ones and experiment with running
similar commands from the command line.

When complete uncomment cron.
