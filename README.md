# Spicule's Traditional Pentaho Data Integration Bundle 

## Overview

This bundle deploys a scalable Pentaho Data Integration server with a MySQL database for quick
and easy data transformation and processing. Data integration is the underpinning of any successful
analytics project and Pentaho Data Integration offers the most user friendly way to do it.

# Usage

Out of the box this bundle provides a single Pentaho Data Integration server alongside a pre configured
MySQL database.

Deploying this bundle:
 
    juju deploy ~spiculecharms/pdi-bundle

### Using a specific PDI version

You can switch between stable, candidate, beta and edge branches within our PDI charm. This will allow
you to run newer but less tested versions of PDI. 

    juju 


## Interacting with the PDI cluster

There are number of ways to run jobs on the PDI cluster both on-demand, scheduled and remotely. 

### Running jobs and transformations on demand

To run a job execute the following:
   

To execute a transformation run this command:



### Scheduling jobs and transformation for execution

You can also schedule regular jobs to run on a repeated basis. To do this run the following command:



### Accessing the Carte server

The carte server provides remote access and monitoring of your PDI cluster and also orchestrates the job
distribution and load when scaling out. 

To set the Carte password run the following:

   
Your Carte server will then be accessible at the master IP address listed in juju status. Your connection
should look similar to the following:

    

# Scale out Usage

Scaling both PDI and MySQL is quick and simple to add new units run:

    juju add-unit pentaho-data-integration

To remove units you can run:

    juju remove-unit pentaho-data-integration


## Known Limitations and Issues



## PDI details

There are a number of good resources available for PDI:

[Penatho community website](https://community.hds.com/community/products-and-solutions/pentaho/)
[Pentaho forums](https://forums.pentaho.com/)

## Further information

For bespoke support and deployment options contact [Spicule](https://spicule.co.uk/contact/)