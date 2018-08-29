# Maven plugins experiment for JDK 9 projects

This is an attempt to enable the use of JDK 9 `--module-path` options in replacement of `--class-path`
when building Maven projects. The new JDK 9 options allow to compile more than one Java module at once.
This capability enables aggregated Javadoc and simplifies the handling of some circular dependency issues,
among others advantages. Another goal is to make more convenient to handle Python code together with Java
code in the same project. However this experiment requires:

* a new directory layout, different than the standard Maven directory layout;
* a modification of standard Maven plugins.

Those requirements are presented in the [wiki](https://github.com/Geomatys/maven-plugins/wiki) page,
together with an example of project structured according the proposed new layout. This GitHub repository
contains clones of standard Maven plugins as Git sub-modules, for hosting the required changes.

## Status

As of August 2018, development has not yet started.
This repository contains only clone of standard Maven plugins.

|     Maven plugin      | Cloned from | Development status |
|-----------------------|-------------|--------------------|
| maven-compiler-plugin |    3.8.0    | not started        |
| maven-javadoc-plugin  |    3.0.1    | not started        |
| maven-jar-plugin      |    3.1.0    | not started        |
| maven-deploy-plugin   |    2.8.2    | not started        |
