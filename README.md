# Jekyll for OpenShift

Template for running jekyll on OpenShift.

## Status

Work in progress, please report issues.

Updated!!

## How to

Your jekyll source should be placed in the lib/ directory. Once you push your code, this quickstart builds the site for you.

## Installation

Create OpenShift application

    rhc app create $name ruby-1.9 --from-source=git://github.com/dmueller2001/jekyll-openshift-quickstart.git

enter the directory

    cd $name

and build your application using Awestruct.

To deploy to OpenShift just push

    git push origin master

Now, your application is available at

    http://$name-$namespace.rhcloud.com

## What it does?

* Install jekyll/dependencies if needed
* Update jekyll/dependencies if possible
* Generate the site to static files

## Tools

* Jekyll
* Phusion Passenger & Apache for serving the files
