commons-text-api Plugin
===================

[![Build Status](https://ci.jenkins.io/job/Plugins/job/commons-text-api-plugin/job/main/badge/icon)](https://ci.jenkins.io/job/Plugins/job/commons-text-api-plugin/job/main/)
[![Contributors](https://img.shields.io/github/contributors/jenkinsci/commons-text-api-plugin.svg)](https://github.com/jenkinsci/commons-text-api-plugin/graphs/contributors)
[![Jenkins Plugin](https://img.shields.io/jenkins/plugin/v/commons-text-api.svg)](https://plugins.jenkins.io/commons-text-api)
[![GitHub release](https://img.shields.io/github/v/tag/jenkinsci/commons-text-api-plugin?label=changelog)](https://github.com/jenkinsci/commons-text-api-plugin/blob/main/CHANGELOG.md)
[![Jenkins Plugin Installs](https://img.shields.io/jenkins/plugin/i/commons-text-api.svg?color=blue)](https://plugins.jenkins.io/commons-text-api)

This plugin provides [Commons Text v1.x](https://commons.apache.org/proper/commons-text/) to Jenkins Plugins.<br>

Version will be "&lt;commons-text version&gt;.&lt;plugin version&gt;", so clear what upstream dependency it is offering and plugin can be patch by "plugin version" if required.

## How to introduce to your plugin

### Plugins directly depending on commons-text

Replace the dependency to `org.apache.commons:commons-text` with the dependency to `commons-text-api`.

* Before:
    ```
    <dependencies>
      ...
      <dependency>
        <groupId>org.apache.commons</groupId>
        <artifactId>commons-text</artifactId>
        <version>1.9</version>
      </dependency>
      ...
    </dependencies>
    ```
* After:
    ```
    <dependencies>
      ...
      <dependency>
        <groupId>io.jenkins.plugins</groupId>
        <artifactId>commons-text-api</artifactId>
        <version>1.9.0</version>
      </dependency>
      ...
    </dependencies>
    ```

### Change Log

#### Version 1.9.0 (June TBC, 2022)
- First release
- Discussed in [[PR#1979](https://github.com/jenkinsci/configuration-as-code-plugin/pull/1979#discussion_r887891629)].
