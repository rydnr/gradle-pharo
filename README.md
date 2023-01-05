= Gradle Pharo =

This repository is meant to be used in Pharo projects that use Gradle as their build tool.

== Usage ==

First, add this repository as a submodule of your Pharo project:

``` sh
git submodule add https://github.com/rydnr/gradle-pharo .gradle-pharo
```

Second, create symlinks:

``` sh
ln -s .gradle-pharo/build.gradle .
```

Third, create the required files with your custom settings:

``` sh
cp .gradle-pharo/gradle.properties.sample gradle.properties
cp .gradle-pharo/gradle-local.properties.sample gradle-local.properties
```

Finally, add your custom settings in /gradle.properties/ and /gradle-local.properties/.
