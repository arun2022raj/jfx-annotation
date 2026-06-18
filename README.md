# JFX Annotations — Maven project

**jfx-annotations** provides runtime annotations for explicit JFX ↔ Java mapping (`@JfxRoot`, `@JfxNode`, `@JfxProperty`, `@JfxArgument`, `@JfxIgnore`).

This is a **standalone** Maven project — sibling of [JFX-MAVEN-PRJECT](../JFX-MAVEN-PRJECT/) (jfx-core) and [jfx-databind-maven-project](../jfx-databind-maven-project/) (jfx-databind).

## Layout

```
jfx-annotations-maven-project/
├── pom.xml                 ← parent POM (jfx-annotations-parent)
└── jfx-annotations/
    ├── pom.xml
    └── src/main/java/com/vstack/jfx/annotations/
```

## Build

No external JFX dependencies — build and install locally:

```bash
cd jfx-annotations-maven-project
mvn clean install
```

Produces `in.co.vstack:jfx-annotations:0.1.1-SNAPSHOT` locally (Maven Central release: `0.1.0`).

## Maven dependency (Maven Central)

```xml
<dependency>
    <groupId>in.co.vstack</groupId>
    <artifactId>jfx-annotations</artifactId>
    <version>0.1.0</version>
</dependency>
```

**jfx-databind** depends on this artifact at compile time. Install annotations before building databind, or use databind’s `bootstrap-deps` profile.

## Annotations

| Annotation | Purpose |
|------------|---------|
| `@JfxRoot("ApiSpec")` | Root `@Tag` in `.jfx` file |
| `@JfxNode("Field")` | Child `@Tag` name |
| `@JfxProperty("mapped_name")` | Property key override |
| `@JfxArgument` | Field for `("…")` argument |
| `@JfxIgnore` | Skip field on read/write |

## License

Licensed under the [Apache License, Version 2.0](LICENSE).

## Security

See [SECURITY.md](SECURITY.md) for how to report vulnerabilities.
