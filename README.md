Apache Syncope overlay to be run in Glassfish.<br/>
Practical implementation of official advices at Syncope [wiki](https://cwiki.apache.org/confluence/display/SYNCOPE/Run+Syncope+in+real+environments).

## How to test ##

This projects assumes that you have
 1. [Apache Maven 3.0](http://maven.apache.org) installed
 1. a running Glassfish instance, listening to port 8080
 1. a MySQL datasource named <code>syncopeDataSource</code> referring to an empty db

#### clone ####

<pre>
$ git clone git://github.com/Tirasa/syncopeOnGlassfish.git
</pre>

#### build ####

<pre>
$ cd syncopeOnGlassfish
$ mvn clean package
</pre>

#### deploy ####

 1. <code>core/target/syncope.war</code>
 1. <code>console/target/syncope-console.war</code>

## Notes ##
 1. Currently on 1.0.8
 1. Not listenig on 8080? Just put the correct port in <code>console/src/main/resources/configuration.properties</code>, re-build and re-deploy

## Need more info? ##
Just drop an [e-mail](mailto:syncope@tirasa.net).
