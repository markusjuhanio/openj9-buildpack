# OpenJ9 Buildpack

This custom buildpack installs [Eclipse OpenJ9 VM](https://www.eclipse.org/openj9) [AdoptOpenJDK11](https://adoptopenjdk.net/).

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
