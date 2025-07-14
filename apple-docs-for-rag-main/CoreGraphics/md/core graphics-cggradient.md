

- Core Graphics
-  CGGradient 

Class

# CGGradient

A definition for a smooth transition between colors for drawing radial and axial gradient fills.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CGGradient
```

## Overview

A gradient defines a smooth transition between colors across an area. A `CGGradient` has a color space, two or more colors, and a location for each color. The color space cannot be a pattern or indexed color space, otherwise it can be any Core Graphics color space (CGColorSpace).

Colors can be provided as component values (such as red, green, blue) or as Core Graphics color objects (CGColor). Component values can vary from 0.0 to 1.0, designating the proportion of the component present in the color.

A location is a normalized value. When it comes time to paint the gradient, Core Graphics maps the normalized location values to the points in coordinate space that you provide.

For more precise control over gradients, see CGShading.

## Topics

### Creating Gradient Instances

init?(colorSpace: CGColorSpace, colorComponents: UnsafePointer&lt;CGFloat>, locations: UnsafePointer&lt;CGFloat>?, count: Int)

Creates a CGGradient object from a color space and the provided color components and locations.

init?(colorsSpace: CGColorSpace?, colors: CFArray, locations: UnsafePointer&lt;CGFloat>?)

Creates a gradient object from a color space and the provided color objects and locations.

### Working with Core Foundation Types

class var typeID: CFTypeID

Returns the Core Foundation type identifier for CGGradient objects.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Utility and Support Classes

class CGDataConsumer

An abstraction for data-writing tasks that eliminates the need to manage a raw memory buffer.

class CGDataProvider

An abstraction for data-reading tasks that eliminates the need to manage a raw memory buffer.

class CGShading

A definition for a smooth transition between colors, controlled by a custom function you provide, for drawing radial and axial gradient fills.

class CGFunction

A general facility for defining and using callback functions.

class CGPattern

A 2D pattern to be used for drawing graphics paths.

