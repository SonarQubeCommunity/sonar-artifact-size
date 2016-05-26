Artifact Size Plugin
====================
[![Build Status](https://api.travis-ci.org/SonarQubeCommunity/sonar-artifact-size.svg)](https://travis-ci.org/SonarQubeCommunity/sonar-artifact-size)

## Description / Features
This plugin is used to measure and record the size of the project artifact, on a dashboard and on a TimeMachine widget.

## Usage
Run a new quality analysis and the metrics will be fed.

By default, on a Maven project, the plugin retrieves the size on its own. Otherwise, a property should be set at the project or module level to pass the path to the artifact.
For example: sonar.artifact.path=target/zip/myCustomArtiact.zip

## Known Limitations
* This plugin requires that a build is run to generate the artifact prior to the SonarQube analysis.
* In a multi-module environment, a property passed to the root pom will be used for modules.
