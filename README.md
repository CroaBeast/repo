# REPO
Repository to host all my public repositories as dependencies.

## Maven / Gradle Installation

To include Takion, CommandFramework, PrismaticAPI, AdvancementInfo, YAML API, or any other module from the project, add the following repository and dependency to your build configuration. Replace `${artifactName}` with the module you want (e.g., `Takion`, `CommandFramework`, `PrismaticAPI`, `AdvancementInfo`, `YAML-API`) and `${version}` with the desired version tag.

### Maven

Add the repository and dependency to your `pom.xml`:

```xml
<repositories>
    <repository>
        <id>croabeast-repo</id>
        <url>https://croabeast.github.io/repo/</url>
    </repository>
</repositories>

<dependencies>
    <dependency>
        <groupId>me.croabeast</groupId>
        <artifactId>${artifactName}</artifactId>
        <version>${version}</version>
        <scope>compile</scope>
    </dependency>
</dependencies>
```

### Gradle

Add the repository and dependency to your `build.gradle`:

```groovy
repositories {
    maven {
        url "https://croabeast.github.io/repo/"
    }
}

dependencies {
    implementation "me.croabeast:${artifactName}:${version}"
}
```

Replace `${artifactName}` and `${version}` with the appropriate module name and version.
