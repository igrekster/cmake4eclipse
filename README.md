[Install...](#installation-instructions)
[![Mailing-list](https://img.shields.io/badge/Mailing-list-blue.svg)](http://groups.google.com/d/forum/cmake4eclipse-users)
[![Build Status](https://travis-ci.org/15knots/cmake4eclipse.svg?branch=master)](https://travis-ci.org/15knots/cmake4eclipse)
[![GitHub issues](https://img.shields.io/github/issues/15knots/cmake4eclipse.svg)](https://github.com/15knots/cmake4eclipse/issues)


# Introduction
The [CMake Wiki](https://cmake.org/Wiki/CMake:Eclipse_UNIX_Tutorial#CMake_with_Eclipse) mentions three options to use CMake with Eclipse.
This Eclipse plugin offers one more option to do that:
It is designed to **automatically** generate buildscripts for the Eclipse CDT managed build system from CMake scripts. 

# Why cmake4eclipse?
Blindly invoked, CMake will generate makefiles (or other build scripts) inside the source tree, cluttering it with lots of files and directories that have to be fleed out from version control: This practice might be ok for simple hello-world-projects, but for larger projects, the CMake developers recommend _You_ to set up a separate directory for building the source.

Annoyingly, these recommended out-of-source-builds impose some tedious tasks on Your co-workers who check out the code and just want to build it:
  1. leave eclipse workbench,
  1. manually fire up a command-line shell,
  1. manually create a directory for the out-of-source-build,
  1. manually change the CWD to that directory,
  1. manually invoke cmake, telling it to generate build scripts, which kind of build scripts you want and where source source files live,
  1. re-enter eclipse workbench, configure the checked out project to use the generated buildscripts.

**Cmake4eclipse** aims to address these tasks: Co-workers can just check out the source and have all the tedious tasks automated.

## Screenshots
Screenshots can be found at the <a href="https://marketplace.eclipse.org/content/cmake4eclipse#group-screenshots" title="Screenshots">Eclipse Marketplace</a>.

## License
The plugin is licensed uner the <a href="http://www.eclipse.org/legal/epl-v10.html">Eclipse Public License Version 1.0 ("EPL")</a>.

# Installation Instructions
The easiest way is to drag this: <a href="http://marketplace.eclipse.org/marketplace-client-intro?mpc_install=2318334" class="drag" title="Drag to your running Eclipse workbench to install cmake4eclipse">
<img class="img-responsive" src="https://marketplace.eclipse.org/sites/all/themes/solstice/_themes/solstice_marketplace/public/images/btn-install.png" alt="Drag to your running Eclipse workbench to install cmake4eclipse" /></a> to your running Eclipse workbench.

Alternatively, **cmake4eclipse** can be installed into Eclipse using the "Install New Software..." dialog and entering the update site URL listed below.

### Update Site
This composite update site contains the latest release as well as selected older releases.
https://raw.githubusercontent.com/15knots/cmake4eclipse/master/releng/comp-update/

---
# Release History
## 1.4.4 (2016-10-05)
### Changes
- Closed #17: CMAKE_EXPORT_COMPILE_COMMANDS parser doesn't recognize g++ as a C++ compiler.

### Repository URL
`jar:https://bintray.com/artifact/download/15knots/p2-zip/cmake4eclipse-1.4.3.zip!/`
### System Requirements
CDT v 8.1.0 or higher and Eclipse v 3.8.0 (Juno) or higher

## 1.4.3 (2016-08-30)
### Changes
- Closed #16: The CMAKE_EXPORT_COMPILE_COMMANDS parser now knows about GCC cross compilers for C and C++ if the compiler executable follows the naming convention of
`<target_triplet>-gcc` or `<target_triplet>-g++`. 

### Repository URL
`jar:https://bintray.com/artifact/download/15knots/p2-zip/cmake4eclipse-1.4.3.zip!/`
### System Requirements
CDT v 8.1.0 or higher and Eclipse v 3.8.0 (Juno) or higher

## 1.4.2 (2016-05-30)
### Changes
- CMAKE_EXPORT_COMPILE_COMMANDS Parser triggers UI update to show newly detected include paths in project explorer view.
- Closed #14: Pass variables given in C++ Build->Environment to the cmake process.

### Repository URL
`jar:https://bintray.com/artifact/download/15knots/p2-zip/cmake4eclipse-1.4.2.zip!/`
### System Requirements
CDT v 8.1.0 or higher and Eclipse v 3.8.0 (Juno) or higher

## 1.4.1 (2016-03-08)
### Changes
- Closes #9: Improve support for code-completion and symbol browsing in CDT source editors.
- Closes #10: Can't install version 1.4.0 in eclipse mars.2 release 4.5.2

### Repository URL
`jar:https://bintray.com/artifact/download/15knots/p2-zip/cmake4eclipse-1.4.1.zip!/`
### System Requirements
CDT v 8.1.0 or higher and Eclipse v 3.8.0 (Juno) or higher

---
## Archived Releases
These releases are made available as a zipped p2 repository. To install, use the "Install New Software..." menu and paste the appropriate repository URL from below into the "Work with" input field.

### 1.3.5 (2015-10-14)
#### Repository URL
`jar:https://bintray.com/artifact/download/15knots/p2-zip/cmake4eclipse-1.3.5.zip!/`
#### System Requirements
CDT v 8.1.0 or higher and Eclipse v 3.8.0 (Juno) or higher

### 1.3.4 (2015-10-09)
#### Repository URL
`jar:https://bintray.com/artifact/download/15knots/p2-zip/cmake4eclipse-1.3.4.zip!/`
#### System Requirements
CDT v 8.1.0 or higher and Eclipse v 3.8.0 (Juno) or higher

### 1.3.3 (2015-05-06)
#### Repository URL
`jar:https://bintray.com/artifact/download/15knots/p2-zip/cmake4eclipse-1.3.3.zip!/`
#### System Requirements
CDT v 8.1.0 or higher and Eclipse v 3.8.0 (Juno) or higher

### 1.3.2 (2015-03-27)
#### Repository URL
`jar:https://googledrive.com/host/0B-QU1Qnto3huZUZ0QUdxM01pR0U/cmake4eclipsecdt-1.3.2.zip!/`
#### System Requirements
CDT v 8.1.0 or higher and Eclipse v 3.8.0 (Juno) or higher

### 1.3.1 (2015-01-21)
#### Repository URL
`jar:https://googledrive.com/host/0B-QU1Qnto3huZUZ0QUdxM01pR0U/cmake4eclipsecdt-1.3.1.zip!/`
#### System Requirements
CDT v 8.1.0 or higher and Eclipse v 3.8.0 (Juno) or higher

### 1.3.0 (2014-12-20)
#### Repository URL
`jar:https://googledrive.com/host/0B-QU1Qnto3huZUZ0QUdxM01pR0U/cmake4eclipsecdt-1.3.0.zip!/`
#### System Requirements
CDT v 8.1.0 or higher and Eclipse v 3.8.0 (Juno) or higher

### 1.1.0 / 1.2.0.201404092022 (2014-04-09)
#### Repository URL
`jar:https://googledrive.com/host/0B-QU1Qnto3huZUZ0QUdxM01pR0U/cmake4eclipsecdt-1.1.0.zip!/`
#### System Requirements
CDT v 8.1.0 or higher and Eclipse v 3.8.0 (Juno) or higher

### 1.0.0 (2014-03-07)
#### Repository URL
`jar:https://googledrive.com/host/0B-QU1Qnto3huZUZ0QUdxM01pR0U/cmake4eclipsecdt-1.0.0.zip!/`
#### System Requirements
 CDT v 8.1.0 or higher and Eclipse v 3.8.0 (Juno) or higher

---
## Ancient Releases
Other revisions can be found at <a href='https://googledrive.com/host/0B-QU1Qnto3huZUZ0QUdxM01pR0U/'>https://googledrive.com/host/0B-QU1Qnto3huZUZ0QUdxM01pR0U/</a> .<br>
Do not forget to add the trailing <b>!/</b> to the repository URL!<br>
