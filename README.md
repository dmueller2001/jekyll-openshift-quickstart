# Awestruct for OpenShift

Template for running awestruct on OpenShift.

## Status

Work in progress, please report issues.

Updated!!

## How to

Your awestruct source should be placed in the lib/ directory. Once you push your code, this quickstart builds the site for you.

## Installation

Create OpenShift application

    rhc app create $name ruby-1.9 --from-source=git://github.com/openshift-quickstart/awestruct-openshift-quickstart.git

enter the directory

    cd $name

and build your application using Awestruct.

To deploy to OpenShift just push

    git push origin master

Now, your application is available at

    http://$name-$namespace.rhcloud.com

## What it does?

* Install awestruct/dependencies if needed
* Update awestruct/dependencies if possible
* Generate the site to static files

## Tools

* Awestruct
* Phusion Passenger & Apache for serving the files
