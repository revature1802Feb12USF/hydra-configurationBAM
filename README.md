# hydra-configuration
Configurations for the Hydra Config Server

## Configuration Design
- The application.yml is the backup generic configuration for services that are not specified.
- Other .yml files are specific for different buisness services.

## Steps to run

1. Download ojdbc8.jar if you don't have it from [here](http://www.oracle.com/technetwork/database/features/jdbc/jdbc-ucp-122-3110062.html)

2. Run Maven install goal
Change <file-location> to location of your jar. 
```
mvn install:install-file -Dfile="<file-location>" -DgroupId=com.oracle -DartifactId=ojdbc8 -Dversion=12.2.0.1 -Dpackaging=jar
```