# **livy**
___

### Description
___

This image runs the  [*Apache Livy*](http://livy.incubator.apache.org./) with Spark on a Centos Linux distribution.

The *latest* tag of this image is build with the latest stable release of Livy and Spark.

You can pull it with:

    docker pull parrotstream/livy


You can also find other images based on different Apache Livy and Spark releases, using a different tag in the following form:

    docker pull parrotstream/livy:[livy-release]-[spark-release]


or in the following form in the case of a Cloudera Spark distribution in CDH:

    docker pull parrotstream/livy:[livy-release]-[spark-release]-[cdh-release]


For example, if you want Apache Livy release 0.2.0 and Spark 1.6.0 in CDH 5.11.1 you can pull the image with:

    docker pull parrotstream/livy:0.2.0-1.6.0-cdh5.11.1


Run with Docker Compose:

    docker-compose -p parrot up


Setting the project name to *parrot* with the **-p** option is useful to share the network created with the containers coming from other Parrot docker-compose.yml configurations.

Once started you'll be able to access the Livy REST Api at:

| **HUE Web GUI**           |**URL**                            |
|:--------------------------|:----------------------------------|
| *Livy REST Api*           | http://localhost:8998             |


### Available tags:

- Apache Livy 0.3.0-1.6.0-cdh5.11.1 ([0.3.0-1.6.0-cdh5.11.1](https://github.com/parrot-stream/docker-livy/blob/0.3.0-1.6.0-cdh5.11.1/Dockerfile))
