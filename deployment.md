# DEPLOYMENT

The sections in this document should be installed in the order they appear.

These instructions assume the reader and/or her team have plenty experience in
UNIX-like OS's administration and some programming knowledge.

Energy Access Explorer is divided into several code-bases to help keep
everything sanitised and modular.

## Base requirements

Installation and configuration of the following are outside the scope of this
document and will be considered "basic knowledge" the a development team should
have.

- nginx (or any other full-featured webserver)
- git, bmake (make BSD syntax), rsync, curl, sh
- a JWT authentication mechanism similar to Auth0

## Database

The database server we use is PostreSQL. An instance is required.

See https://github.com/energyaccessexplorer/database to get specific
instructions.

## API

The API is delegated [PostgREST](https://postgrest.org/en/stable/).

Setting up PostgREST is fairly straight forward. Some optional functionality,
wrappers/scripts (used by Energy Access Explorer) are here:
https://github.com/energyaccessexplorer/api

Setting up PostgREST + JWT authentication depends on the authentication service
(potentially a 3rd party like Auth0) and thus outsite the scope this document.

## Website

See https://github.com/energyaccessexplorer/website to get specific
instructions.

## Tool

The tool requires the website above to be up and running since they share some
components which are hosted there.

See https://github.com/energyaccessexplorer/tool to get specific
instructions.

## Paver

This project is optional but does most of the GIS heavy lifting.

See https://github.com/energyaccessexplorer/paver to get specific
instructions.

## Offroad

This project is optional.

See https://github.com/energyaccessexplorer/offroad to get specific
instructions.

## Departer

This project is optional.

See https://github.com/energyaccessexplorer/departer to get specific
instructions.
