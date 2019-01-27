# minecraft-datapacks

[![Build Status](https://travis-ci.org/rremer/minecraft-datapacks.svg?branch=master)](https://travis-ci.org/rremer/minecraft-datapacks)

A collection of composable datapacks for Minecraft.

## Building

```sh
mvn clean install
```

## Modules

Overviow of the Maven reactor modules present in this project.

### schema

This module contains the datapack JSON schemas. Perhaps Mojang will provide these one day, so we use maven resource filtering to plug in the schema URL.
