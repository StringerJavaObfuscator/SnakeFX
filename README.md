## Java FX App Protection

This is a fork of a simple Java FX game to demonstrate Stringer Obfuscator using for similar apps.

## Description
- https://jfxstore.com/stringer/docs#gradle-plugin

## Requirements
- Stringer Standard or Enterpise with a valid license
- Gradle (optional)

## Configuring 

- Install Stinger and Stringer Gradle plugin to local Maven repository::

```
mvn install:install-file -Dfile=`pwd`/stringer.jar -DpomFile=`pwd`/stringer.pom
mvn install:install-file -Dfile=`pwd`/stringer-annotations.jar -DpomFile=`pwd`/stringer-annotations.pom
mvn install:install-file -Dfile=`pwd`/stringer-gradle-plugin.jar -DpomFile=`pwd`/stringer-gradle-plugin.pom
```

## Build the game
The game is created with Java version 8 so you will need to have Java 8 installed to be able to build the project. 
The project is based on the build system [gradle](http://http://www.gradle.org/). 

To build the project type `gradle build`.

## Create Executables

A runnable JAR can be created with `gradle shadowJar`. The JAR file is then located under `build/libs/SnakeFX-all.jar`

## Stringer Protection Examples
This game uses the [MvvmFX](http://www.lestard.eu/projects/mvvmfx/) framework.
If you want to encrypt resources (css, fxml files) by Stringer, you should add classes of this framework to the project's jar file and exclude the library from the /libs folder of project distribution archive.
Examples below show Stringer protection for classes and resources.

### A class without protection 
![Not Protected Class](img/class.png)

### The class protected by Stringer
![Protected Class](img/class_protected.png)

### A resource (fxml file) without protection 
![Not Protected Resource](img/fxml.png)

### The resource protected by Stringer
![Protected Resource](img/fxml_protected.png)

### A resource (fxml file) without protection 
![Not Protected Resource](img/css.png)

### The resource protected by Stringer
![Protected Resource](img/css_protected.png)

### A service class created by Stringer for the resources above
![Service Class](img/class_service.png)

# SnakeFX
This is a clone of the old mobile phone game "Snake".
It was created as an example project to learn *JavaFX*.

![screenshot](screenshot.png)

The object of the game is simple: You are controlling a snake that likes to eat
food. Every time the snake eats some food it grows a little bit. You may not bite yourself in the tail or you are game over. There are no walls in this game so when you move outside of one side of the screen you appear again on the other side of the screen.

### Play the Game

You can download a runnable JAR from the [release-secton](https://github.com/lestard/SnakeFX/releases/download/v0.1.0/snakefx.0.1.0.jar) of github. To run the game you need Oracles Java version 8 installed.



