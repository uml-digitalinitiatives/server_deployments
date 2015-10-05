# Manitobia

## Overview:

Manitobia consists of a single virtual server and storage is a 8 GB NFS mount.

* RedHat Enterprise Linux Server release 5.11 (Tikanga)
* 1 CPUs
* 2 GB RAM

### Tomcat webapps:

* Apache Cocoon 
* Apache Solr

### Software versions:

* Apache: 2.2.3
* Java: 1.6.0_26 (Oracle)
* jQuery: 1.4
* Solr: 1.4.2
* Cocoon: 2.1

### Settings:

* JAVA_OPTS="-XX:+UseConcMarkSweepGC -XX:SurvivorRatio=8 -XX:+OptimizeStringConcat -XX:+UseCompressedStrings -XX:+CMSClassUnloadingEnabled -XX:+CMSScavengeBeforeRemark -XX:+UseParNewGC -Dcatalina.ext.dirs=$CATALINA_HOME/shared/lib:$CATALINA_HOME/common/lib -Dsolr.solr.home=/var/solr -Djava.awt.headless=true -d64 -Xmx1536m -XX:MaxPermSize=512m -server"
