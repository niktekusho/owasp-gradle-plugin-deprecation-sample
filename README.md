# Reproduction case for the issue XXX

This repository contains the reproduction case for the issue xxx.

When running the dependency analyzer plugin,  Gradle warns about the resolution of deprecated configurations. Gradle 7 will not set up these configurations. 

```
The archives configuration has been deprecated for resolution. This will fail with an error in Gradle 7.0. Please resolve the compileClasspath or runtimeClasspath configuration instead. Consult the upgrading guide for further information: https://docs.gradle.org/6.4/userguide/upgrading_version_5.html#dependencies_should_no_longer_be_declared_using_the_compile_and_runtime_configurations
```

## Instructions

### Clone repository

```sh
 $ git clone https://github.com/niktekusho/xxx
``` 

### Build the multi-project to check for errors

```sh
 $ ./gradlew build --parallel
``` 

### Run the dependency analyzer plugin

```sh
 $ ./gradlew dependencyCheckAnalyze
``` 
