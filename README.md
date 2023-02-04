# Maven & Java skeleton

This repository contains a starting point for Java projects.

It configures the compiler to use UTF-8, Java 17, and enables reflection on parameters. It also shows deprecated APIs
and fails on warnings. It contains the [Maven wrapper](https://maven.apache.org/wrapper/).

It includes SLF4J as logging API, logback (with ISO8601 timestamps) as logging backend, JUnit 5 for testing, and AssertJ
for test assertions.

It copies the dependencies to `target/lib`, and configures the JAR file with a main class and a classpath, so that the
resulting JAR can be run with `java -jar`.

## How to use

Download [the latest version here](https://github.com/phxql/java-maven-skeleton/archive/master.zip), unzip it,
change `<groupId>` and `<artifactId>` and start hacking.

If you're changing the main class (rename the class or move the package), make sure to update `mainClass` configuration
from the `maven-jar-plugin` in the `pom.xml`.

## Building

Run `./mvnw clean package` and check the `target` folder.

## Distributing your project

Copy the JAR file and the `lib/` directory from the `target` folder.

## License

Licensed under [CC0](https://creativecommons.org/publicdomain/zero/1.0/) - do whatever you want with it.
