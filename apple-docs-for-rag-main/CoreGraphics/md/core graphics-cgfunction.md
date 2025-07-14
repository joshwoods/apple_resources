

- Core Graphics
-  CGFunction 

Class

# CGFunction

A general facility for defining and using callback functions.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CGFunction
```

## Overview

These functions can take an arbitrary number of floating-point input values and pass back an arbitrary number of floating-point output values.

Core Graphics uses function objects to implement shadings. CGShading describes the parameters and semantics required for the callbacks used by function objects.

## Topics

### Creating Function Objects

init?(info: UnsafeMutableRawPointer?, domainDimension: Int, domain: UnsafePointer&lt;CGFloat>?, rangeDimension: Int, range: UnsafePointer&lt;CGFloat>?, callbacks: UnsafePointer&lt;CGFunctionCallbacks>)

Creates a Core Graphics function.

### Callbacks

struct CGFunctionCallbacks

A structure that contains callbacks needed by a `CGFunctionRef` object.

typealias CGFunctionEvaluateCallback

Performs custom operations on the supplied input data to produce output data.

typealias CGFunctionReleaseInfoCallback

Performs custom clean-up tasks when Core Graphics deallocates a `CGFunctionRef` object.

### Working with Core Foundation Types

class var typeID: CFTypeID

Returns the type identifier for Core Graphics function objects.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Related Documentation

Quartz 2D Programming Guide

### Utility and Support Classes

class CGDataConsumer

An abstraction for data-writing tasks that eliminates the need to manage a raw memory buffer.

class CGDataProvider

An abstraction for data-reading tasks that eliminates the need to manage a raw memory buffer.

class CGShading

A definition for a smooth transition between colors, controlled by a custom function you provide, for drawing radial and axial gradient fills.

class CGGradient

A definition for a smooth transition between colors for drawing radial and axial gradient fills.

class CGPattern

A 2D pattern to be used for drawing graphics paths.

