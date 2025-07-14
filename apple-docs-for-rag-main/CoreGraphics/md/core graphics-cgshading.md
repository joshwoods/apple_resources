

- Core Graphics
-  CGShading 

Class

# CGShading

A definition for a smooth transition between colors, controlled by a custom function you provide, for drawing radial and axial gradient fills.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CGShading
```

## Overview

Shading means to fill using a smooth transition between colors across an area. You create a shading using a custom function with a CGFunction instance. To paint with a Core Graphics shading, you call drawShading(_:). This function fills the current clipping path using the specified color gradient, calling your parametric function repeatedly as it draws.

An alternative to using a `CGShading` instance is to use the CGGradient type. For applications that run in macOS 10.5 and later, `CGGradient` objects are much simpler to use.

## Topics

### Creating Shading Objects

init?(axialSpace: CGColorSpace, start: CGPoint, end: CGPoint, function: CGFunction, extendStart: Bool, extendEnd: Bool)

Creates a shading object to use for axial shading.

init?(radialSpace: CGColorSpace, start: CGPoint, startRadius: CGFloat, end: CGPoint, endRadius: CGFloat, function: CGFunction, extendStart: Bool, extendEnd: Bool)

Creates a shading object to use for radial shading.

### Working with Core Foundation Types

class var typeID: CFTypeID

Returns the Core Foundation type identifier for Core Graphics shading objects.

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

class CGGradient

A definition for a smooth transition between colors for drawing radial and axial gradient fills.

class CGFunction

A general facility for defining and using callback functions.

class CGPattern

A 2D pattern to be used for drawing graphics paths.

