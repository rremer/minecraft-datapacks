# minecraft-datapacks

[![Build Status](https://img.shields.io/travis/rremer/minecraft-datapacks)](https://travis-ci.org/rremer/minecraft-datapacks)
[![Maven Central](https://img.shields.io/nexus/r/com.github.rremer/minecraft-datapacks?server=https%3A%2F%2Foss.sonatype.org)](https://search.maven.org/artifact/com.github.rremer/minecraft-datapacks/1.13.2-1/jar)
[![License](https://img.shields.io/github/license/rremer/minecraft-datapacks)](https://opensource.org/licenses/MIT)
[![Keybase PGP](https://img.shields.io/keybase/pgp/rremer)](https://keybase.io/rremer/pgp_keys.asc)

A collection of composable datapacks for Minecraft.

## Building

```sh
mvn clean install
```

## Modules

Overviow of the Maven reactor modules present in this project.

### moar-dyes

More recipes to color variations for blocks and dyes.

## Releasing

Ensure your gpg key is installed and ```settings.xml``` is updated with id oss.sonatype.org [per their instructions].

```sh
mvn versions:set -DnewVersion=1.13.2-2
mvn clean deploy -Dparameter.gpg.skip=false
```

### Versioning

A version number of this project's artifacts is built as ```<minecraft.version>-<project.version>```, where:
* ```minecraft.version``` is a version of minecraft (1.13.2, 1.14.4, ...)
* ```project.version``` is an increment for this project to release against a version of minecraft (1,2,3, ...)

[per their instructions]:https://central.sonatype.org/pages/apache-maven.html
