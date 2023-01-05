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
ln -s .gradle-pharo/run-pharo-in-docker .pharo
ln -s .gradle-pharo/gradle-local.properties.sample .
```

Third, create the required files with your custom settings:

``` sh
cp .gradle-pharo/gradle.properties.sample gradle.properties
cp .gradle-pharo/gradle-local.properties.sample gradle-local.properties
cp .gradle-pharo/settings.gradle.sample settings.gradle
cp .gradle-pharo/gitignore.sample .gitignore
```

Finally, add your custom settings in /gradle.properties/, /settings.gradle/ and /gradle-local.properties/.
