# Reaper [![Dev Build](https://github.com/ruViolence/Reaper/actions/workflows/dev-build.yml/badge.svg)](https://github.com/ruViolence/Reaper/actions/workflows/dev-build.yml)

Fork of Paper for 1.12.2 with some performance tweaks, bug fixes and improvements.

## How To (Server Admins)

Reaper uses the same paperclip jar system that Paper uses.

You can download the latest build of Reaper by going [here](https://github.com/ruViolence/Reaper/releases/latest).

## How To (Plugin Developers)

Maven repository:
```xml
<repository>
    <id>github-ruviolence-reaper</id>
    <name>GitHub ruViolence Apache Maven Packages</name>
    <url>https://maven.pkg.github.com/ruViolence/Reaper</url>
</repository>
```

Reaper-API maven dependency:
```xml
<dependency>
    <groupId>com.github.ruviolence</groupId>
    <artifactId>reaper-api</artifactId>
    <version>1.12.2-R0.1-SNAPSHOT</version>
    <scope>provided</scope>
</dependency>
```

Reaper-Server maven dependency:
```xml
<dependency>
    <groupId>com.github.ruviolence</groupId>
    <artifactId>reaper</artifactId>
    <version>1.12.2-R0.1-SNAPSHOT</version>
    <scope>provided</scope>
</dependency>
```