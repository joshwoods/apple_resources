

- Core Image
-  CIFilterConstructor 

Protocol

# CIFilterConstructor

A general interface for objects that produce CIFilter instances.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
protocol CIFilterConstructor
```

## Overview

Objects implementing this protocol are called *filter constructors*—they produce new instances of `CIFilter` subclasses when filters are requested by name. You can create a filter constructor to provide new, custom filters that other Core Image clients can discover using the `CIFilter` class. Normally, you create and register custom filters by packaging them as Image Units (see Packaging and Loading Image Units), but you can use this protocol to provide new filters within your app that are compositions of existing filters.

To provide custom filters using this protocol, you must:

1.  Create your custom filters as `CIFilter` subclasses.

2.  Create a class that implements this protocol to vend instances of the appropriate `CIFilter` subclasses when requested.

3.  Call the `CIFilter` class method registerName(_:constructor:classAttributes:) for each custom filter, providing the filter’s name, an instance of your filter constructor class, and information about the filter’s attributes.

## Topics

### Providing Filter Objects

func filter(withName: String) -> CIFilter?

Returns a filter object specified by name.

**Required**

## Relationships

### Conforming Types

- CIFilterGenerator

## See Also

### Image Units

class CIPlugIn

The mechanism for loading image units in macOS.

class CIFilterGenerator

An object that creates and configures chains of individual image filters.

protocol CIPlugInRegistration

The interface for loading Core Image image units.

