

- Application Services
- ColorSync Manager
-  Profile Classes 

# Profile Classes

Specify profile class enumerations.

## Overview

The ColorSync Manager supports seven classes, or types, of profiles.

A profile creator specifies the profile class in the profile header’s `profileClass` field. For a description of the profile header, see CM2Header. This enumeration defines the profile class signatures.

## Topics

### Constants

var cmInputClass: Int

An input device profile defined for a scanner.

var cmDisplayClass: Int

A display device profile defined for a monitor.

var cmOutputClass: Int

An output device profile defined for a printer.

var cmLinkClass: Int

A device link profile.

var cmAbstractClass: Int

An abstract profile.

var cmColorSpaceClass: Int

A color space profile.

var cmNamedColorClass: Int

A named color space profile.

