---
title: "Project Apollo: App Structure"
date: 2024-03-05T22:48:22Z
categories: ["coding"]
tags: ["apollo", "software", "development", "music", "detection", "java"]
draft: true
---

In the [first blog post]({{< ref "/coding/project-apollo-the-foundations" >}} "first blog post") of the Apollo project, I suggested that I would be using Java for the project as it's a familiar language to me, and as I would like to deepen my knowledge of Java, it feels like a good candidate. I am aware that there are likely more lightweight/faster/efficient languages/frameworks/tools to use but this time around at least its Java!

I've been thinking about all the possible things that I want to do with this project. However, I am going to embrace an approach where I just get something working, so I can solve the core problem and then follow up with supporting structures. This means my first target is:

> Create a service that takes an audio file and converts it to a structure that can be analysed for comparison purposes.

### Step one: Create the project
I'm using a Maven project structure here with the following POM file:

```xml {lineNos=inline tabWidth=2}
<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
    <modelVersion>4.0.0</modelVersion>

    <groupId>dev.bensheppard</groupId>
    <artifactId>project-apollo</artifactId>
    <version>0.0.1-SNAPSHOT</version>

    <properties>
        <spring-boot.version>3.2.1</spring-boot.version>
        <maven.compiler.source>21</maven.compiler.source>
        <maven.compiler.target>21</maven.compiler.target>
        <project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
    </properties>

    <dependencies>
        <dependency>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-starter-web</artifactId>
            <version>${spring-boot.version}</version>
        </dependency>
    </dependencies>
</project>
```

