# tp-demo-standalone-parent

Standalone parent POM for [tp-demo](https://github.com/jaimegag/tp-demo), kept in its own repository.

- Coordinates: `com.example:tp-demo-standalone-parent:1.0.0`
- Extends `spring-boot-starter-parent` 2.7.11
- Sets `java.version` (11) and `spring-boot.version`
- Child projects inherit `spring-boot-starter-actuator`

## Install

```bash
mvn install
```

Child projects reference it by coordinates with an empty `relativePath`:

```xml
<parent>
    <groupId>com.example</groupId>
    <artifactId>tp-demo-standalone-parent</artifactId>
    <version>1.0.0</version>
    <relativePath/>
</parent>
```
