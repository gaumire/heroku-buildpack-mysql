Heroku buildpack: MySQL
========================

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks) for heroku apps, that require msyql binaries on the dynos itself. The buildpack is supposed to be a supplement to the existing buildpacks available.


Usage
-----

Example usage:

    $ heroku buildpacks:add https://github.com/gaumire/heroku-buildpack-mysql

    $ git push heroku master
    ...
    remote: Compressing source files... done.
    remote: Building source:
    remote: 
    remote: -----> Fetching custom git buildpack... done
    remote: -----> Mysql 5.1 app detected
    remote: -----> Installing Mysql 5.1
    remote: -----> Downloading minimized tarball
    remote: --2015-06-13 05:09:14--  https://raw.githubusercontent.com/gaumire/mysql-binary/master/mysql.tar.gz
    remote: Resolving raw.githubusercontent.com (raw.githubusercontent.com)... 199.27.76.133
    remote: Connecting to raw.githubusercontent.com (raw.githubusercontent.com)|199.27.76.133|:443... connected.
    remote: HTTP request sent, awaiting response... 200 OK
    remote: Length: 6575998 (6.3M) [application/octet-stream]
    remote: Saving to: ‘mysql.tar.gz’
    ...
