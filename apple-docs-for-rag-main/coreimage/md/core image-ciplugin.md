

- Core Image
-  CIPlugIn 

Class

# CIPlugIn

The mechanism for loading image units in macOS.

macOS 10.4+

``` source
class CIPlugIn : NSObject
```

## Overview

An image unit is an image processing bundle that contains one or more Core Image filters. Th`e.plugin` extension indicates one or more filters packaged as an image unit.

Note

Starting in macOS 10.15, loading executable CIFilter plugins is deprecated.

## Topics

### Loading Plug-ins

class func loadNonExecutablePlugIns()

Scans directories for plugins.

class func loadNonExecutablePlugIn(URL!)

Loads a non-executable plug-in specified by its URL.

### Deprecated

class func loadAllPlugIns()

Scans directories for files that have the `.plugin` extension and then loads the image units.

Deprecated

class func load(URL!, allowExecutableCode: Bool)

Loads filters from an image unit that have the appropriate executable status.

Deprecated

## Relationships

### Inherits From

- NSObject

## See Also

### Image Units

class CIFilterGenerator

An object that creates and configures chains of individual image filters.

protocol CIPlugInRegistration

The interface for loading Core Image image units.

protocol CIFilterConstructor

A general interface for objects that produce CIFilter instances.

