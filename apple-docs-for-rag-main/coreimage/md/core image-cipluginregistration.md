

- Core Image
-  CIPlugInRegistration 

Protocol

# CIPlugInRegistration

The interface for loading Core Image image units.

macOS 10.4+

``` source
protocol CIPlugInRegistration
```

## Overview

The principal class of an image unit—a loadable bundle containing custom Core Image filters for macOS—must support this protocol.

## Topics

### Initializing Plug-ins

func load(UnsafeMutableRawPointer!) -> Bool

Loads and initializes an image unit, performing custom tasks as needed.

**Required**

## See Also

### Image Units

class CIPlugIn

The mechanism for loading image units in macOS.

class CIFilterGenerator

An object that creates and configures chains of individual image filters.

protocol CIFilterConstructor

A general interface for objects that produce CIFilter instances.

