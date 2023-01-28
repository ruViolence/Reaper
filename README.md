# Reaper [![Dev Build](https://github.com/ruViolence/Reaper/actions/workflows/dev-build.yml/badge.svg)](https://github.com/ruViolence/Reaper/actions/workflows/dev-build.yml)

Another Paper 1.12.2 fork with some performance enhancements, bug fixes, and improvements.

## Support limitation

I created this fork for myself and I use it on my server.
Therefore, it is of little importance to me if it lacks certain features that others may require.
If you are dissatisfied with this fork, there are many other forks available on the internet.
You may also create your own fork and patch it as you wish.
If there are any bugs in the fork, please report them in the [issues](https://github.com/ruViolence/Reaper/issues),
but there is no guarantee that I will take the time to address them if they do not greatly concern me.

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