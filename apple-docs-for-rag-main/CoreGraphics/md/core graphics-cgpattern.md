

- Core Graphics
-  CGPattern 

Class

# CGPattern

A 2D pattern to be used for drawing graphics paths.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CGPattern
```

## Overview

Core Graphics tiles the pattern cell for you, based on parameters you specify when you call init(info:bounds:matrix:xStep:yStep:tiling:isColored:callbacks:).

To create a dashed line, see CGContextSetLineDash.

## Topics

### Creating a Pattern

init?(info: UnsafeMutableRawPointer?, bounds: CGRect, matrix: CGAffineTransform, xStep: CGFloat, yStep: CGFloat, tiling: CGPatternTiling, isColored: Bool, callbacks: UnsafePointer&lt;CGPatternCallbacks>)

Creates a pattern object.

### Callbacks

struct CGPatternCallbacks

A structure that holds a version and two callback functions for drawing a custom pattern.

typealias CGPatternDrawPatternCallback

Draws a pattern cell.

typealias CGPatternReleaseInfoCallback

Release private data or resources associated with the pattern.

### Constants

enum CGPatternTiling

Different methods for rendering a tiled pattern.

### Working with Core Foundation Types

class var typeID: CFTypeID

Returns the type identifier for Core Graphics patterns.

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

class CGFunction

A general facility for defining and using callback functions.

