
##This is a WIP

We're trying to create a Spark Maven Archetype

First you build and install the archetype

```mvn clean install```

Then the command below should build a scaffolding of a Spark Application

```
mkdir example

cd example

mvn archetype:generate -B     -DarchetypeCatalog=archetype-catalog.xml -DarchetypeGroupId=org.gatesfoundation     -DarchetypeArtifactId=scala-archetype-dataanalytics   -DarchetypeVersion=0.13     -DgroupId=org.gatesfoundation -DartifactId=DSApp -Dversion=0.1-SNAPSHOT -Dpackage=org.gatesfoundation.dataanalytics
```

Then if all goes well there should be a project setup in the example folder.  Here's the output
```
[INFO] Scanning for projects...
[INFO]                                                                         
[INFO] ------------------------------------------------------------------------
[INFO] Building Maven Stub Project (No POM) 1
[INFO] ------------------------------------------------------------------------
[INFO] 
[INFO] >>> maven-archetype-plugin:2.4:generate (default-cli) > generate-sources @ standalone-pom >>>
[INFO] 
[INFO] <<< maven-archetype-plugin:2.4:generate (default-cli) < generate-sources @ standalone-pom <<<
[INFO] 
[INFO] --- maven-archetype-plugin:2.4:generate (default-cli) @ standalone-pom ---
[INFO] Generating project in Batch mode
[INFO] No catalog defined. Using internal catalog
[WARNING] Archetype not found in any catalog. Falling back to central repository (http://repo.maven.apache.org/maven2).
[WARNING] Use -DarchetypeRepository=<your repository> if archetype's repository is elsewhere.
[INFO] ----------------------------------------------------------------------------
[INFO] Using following parameters for creating project from Archetype: scala-archetype-dataanalytics:0.13
[INFO] ----------------------------------------------------------------------------
[INFO] Parameter: groupId, Value: org.gatesfoundation
[INFO] Parameter: artifactId, Value: DSApp
[INFO] Parameter: version, Value: 0.1-SNAPSHOT
[INFO] Parameter: package, Value: org.gatesfoundation.dataanalytics.example
[INFO] Parameter: packageInPathFormat, Value: com/sensus/dataanalytics/example
[INFO] Parameter: package, Value: org.gatesfoundation.dataanalytics.example
[INFO] Parameter: version, Value: 0.1-SNAPSHOT
[INFO] Parameter: groupId, Value: org.gatesfoundation
[INFO] Parameter: artifactId, Value: DSApp
[INFO] project created from Archetype in dir: /home/vagrant/time-series-libraries/MavenArchetype/example/DSApp
```
