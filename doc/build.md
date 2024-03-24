
# Build

## Create a JAR, without assembling executable binaries nor build the web console

```shell
mvn clean package -DskipTests
```

## Create a JAR, only contains the web console

```shell
mvn clean package -DskipTests -P build-web-console
```

## Create a executable binaries

```shell
mvn clean package -DskipTests -P build-web-console,build-binaries
```

## Install

When run `mvn install`, should run `mvn clean` to delete `target` folder.