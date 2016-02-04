# OpenShift-SalesPlatform

[![Join the chat at https://gitter.im/zirf0/openshift-salesplatform-example](https://badges.gitter.im/zirf0/openshift-salesplatform.svg)](https://gitter.im/zirf0/openshift-salesplatform-example?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

SalesPlatform is a fork of VtigerCRM adapted for Russian Federation. Version 6.4.0
# Setup


1) <a href="https://www.openshift.com/app/account/new">Create</a> an account at https://www.openshift.com
2) Install git, ruby <a href=""https://developers.openshift.com/en/getting-started-overview.html>rhc</a> 
3) Create a php application with mysql:

    $ rhc app create spexample php-5.3 mysql-5.5 

4) Add this upstream repo

    $ cd spexample
    $ git remote add upstream -m master git://github.com/zirf0/openshift-salesplatform-example.git
    $ git pull -s recursive -X theirs upstream master

5) Then push the repo upstream

    $ git push

6) That's it, you can now checkout your application at:

    http://spexample-$yourdomain.rhcloud.com

7) Follow installatin procedure

8) Customer portal is avaliable at http://sp-$yourdomain.rhcloud.com/sd

# TODO

1. Take a rest.
2. Add OpenShift-specific documentation
