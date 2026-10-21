> **Deprecated.** This plugin follows the plugin architecture of 2023 and no longer
> builds against the current LabBook Connect: the Analyzer interface has changed since.
> Do not use it as a starting point for a new plugin.

## Where to look instead

- The training material of LabBook Connect, in
  [doc/formation_LabBook_Connect](https://github.com/fondationmerieux/labbook_connect/tree/master/doc/formation_LabBook_Connect),
  which describes the plugin contract, the configuration files and the ASTM and HL7 plugins.
- The plugins in use, as examples:
  [GeneXpert](https://github.com/fondationmerieux/labbook_connect_plugin_genexpert) and
  [Sysmex](https://github.com/fondationmerieux/labbook_connect_plugin_sysmex).

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

# Changes

You can have a look at [CHANGELOG.md](CHANGELOG.md) for changes to the program.

# Contributing

We happily accept contributions but we opened this repository only very recently so we have a long way to go to make contributing easy.

Feel free to open issues when things are confused.

# Licence

[GNU General Public License v2.0](LICENSE.md)
