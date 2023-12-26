# Project

LabBook Connect Plugin Demo is a demo analyzer plugin for [LabBook Connect](https://github.com/fondationmerieux/labbook_connect).

Analyzer plugins convert the HL7v2 messages described in the transactions of the
[IHE-LAW profile](https://wiki.ihe.net/index.php/Laboratory_Analytical_Workflow_Profile)
into messages specific to the type of analyzer.

LabBook Connect Plugins are developped in java.

They implement an interface that is invoked by LabBook Connect.

# Requirements

- linux
- podman
- make
- git

For development:

- java
- eclipse

# Development environment

The Eclipse 4.29.0 (2023-09) plugin and openjdk 21 were used for this project.

Please see `doc/dependencies.md`.

# Installation and usage

Clone the repository

~~~
git clone https://github.com/fondationmerieux/labbook_connect_plugin_demo.git
~~~

Copy the `AnalyzerDemo.jar` file into the `plugin` directory of the LabBook Connect project.

## Plugin API

The plugin must implement the interface described in the `src/plugin/Analyzer.java` file.
Please see the comments in the [file](src/plugin/Analyzer.java) for details.

The plugin can use the functions whose signatures are provided in the `src/plugin/Connect_util.java`
[file](src/plugin/Connect_util.java) to communicate with LabBook Connect.
Please see the LabBook Connect project for the implementation of these functions.

# Changes

You can have a look at [CHANGELOG.md](CHANGELOG.md) for changes to the program.

# Contributing

We happily accept contributions but we opened this repository only very recently so we have a long way to go to make contributing easy.

Feel free to open issues when things are confused.

# Licence

[GNU General Public License v2.0](LICENSE.md)
