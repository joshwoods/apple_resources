

- Installer JS
-  System 

# System

An object that provides access to information about the target host.

## Overview

This object is accessed using the `system` global variable.

## Topics

### Accessing System Information

sysctl

Provides the result of a `sysctlbyname()` call using the given selector.

users.desktopSessionCount

The number of logged-in users.

version

A dictionary (associative array) with information about the current system version.

### Accessing Application Information

applications

An object providing methods to obtain information about running applications.

### Accessing Files

files

An object providing file-access methods.

### Accessing IORegistry

ioregistry

An object providing access to the IOKit registry.

### Accessing Defaults

defaults

A dictionary representing the defaults system.

### Accessing Object Properties

propertiesOf

Provides an array containing the properties of a given object.

### Comparing Version Number Strings

compareVersions

Provides the result of comparing two given version strings (for example, `'10.3.1'` and `'10.4'`).

### Internationalizing Distributions

localizedString

Provides the localized string in the installation package for the current locale for a given key.

localizedStringWithFormat

Provides the formatted localized string in the installation package for the current locale, for a given key and a set of additional arguments.

### Logging

log

Generates an Installer log entry with the `JS:` prefix.

### Running Programs

run

Launches a given program in the `Resources` directory of the installation package.

runOnce

Launches a given program in the `Resources` directory of the installation package, if it has not been run already.

### Legacy Methods

Migrate your code away from these methods.

gestalt

Provides gestalt information that corresponds to the given selector.

localizedStandardString

Provides the localized standard string in the installation package for the current locale for a given key.

localizedStandardStringWithFormat

Provides the formatted localized standard string in the installation package for the current locale, for a given key and a set of additional arguments.

