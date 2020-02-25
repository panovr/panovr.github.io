---
layout: post
title: Example Maven pom.xml for Java application
date:   2020-02-25 20:50:00
categories: Java
---

## Example Maven pom.xml for Java application

This is an example Maven pom.xml for building Java application with Oracle JDK13:

```
<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
    <modelVersion>4.0.0</modelVersion>

    <groupId>org.example</groupId>
    <artifactId>demo</artifactId>
    <version>1.0-SNAPSHOT</version>

    <properties>
        <project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
        <maven.compiler.source>13</maven.compiler.source>
        <maven.compiler.target>13</maven.compiler.target>
    </properties>

    <build>
        <plugins>
            <plugin>
                <groupId>org.apache.maven.plugins</groupId>
                <artifactId>maven-jar-plugin</artifactId>
                <version>3.2.0</version>
                <configuration>
                    <archive>
                        <manifest>
                            <addClasspath>true</addClasspath>
                            <mainClass>org.example.Demo</mainClass>
                        </manifest>
                    </archive>
                </configuration>
            </plugin>
        </plugins>
    </build>
</project>
```

### Reference
[Apache Maven Compiler Plugin](http://maven.apache.org/plugins/maven-compiler-plugin/index.html)
[Apache Maven Compiler Plugin Usage](http://maven.apache.org/plugins/maven-compiler-plugin/examples/set-compiler-source-and-target.html)
[Apache Maven Compiler Plugin Repo](https://mvnrepository.com/artifact/org.apache.maven.plugins/maven-compiler-plugin)
[Apache Maven JAR Plugin](https://maven.apache.org/plugins/maven-jar-plugin/)
[Make The Jar Executable](http://maven.apache.org/shared/maven-archiver/examples/classpath.html#Make)
[Apache Maven JAR Plugin Repo](https://mvnrepository.com/artifact/org.apache.maven.plugins/maven-jar-plugin)
