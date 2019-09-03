# OpenJ9 Buildpack

This buildpack installs the [AdoptOpenJDK11](https://adoptopenjdk.net) with [Eclipse OpenJ9](https://www.eclipse.org/openj9/).

# Usage
Replace the default Heroku Java buildpack

```
$ heroku buildpacks:set https://github.com/olnq/openj9-buildpack.git 
$ heroku buildpacks:add heroku/java  
$ git push heroku master
```

# Customizing

Create a file
**system.properties**
at the root of your project with the following content

```
adoptopenjdk.version=<version>  
adoptopenjdk.release=<release>
```  
