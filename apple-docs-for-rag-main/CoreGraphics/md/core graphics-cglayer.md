

- Core Graphics
-  CGLayer 

Class

# CGLayer

An offscreen context for reusing content drawn with Core Graphics.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CGLayer
```

## Topics

### Creating Layer Objects

init?(CGContext, size: CGSize, auxiliaryInfo: CFDictionary?)

Creates a layer object that is associated with a graphics context.

### Examining a Layer

var context: CGContext?

Returns the graphics context associated with a layer object.

var size: CGSize

Returns the width and height of a layer object.

### Working with Core Foundation Types

class var typeID: CFTypeID

Returns the unique type identifier used for CGLayer objects.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### 2D Drawing

class CGContext

A Quartz 2D drawing environment.

class CGImage

A bitmap image or image mask.

class CGPath

An immutable graphics path: a mathematical description of shapes or lines to be drawn in a graphics context.

class CGMutablePath

A mutable graphics path: a mathematical description of shapes or lines to be drawn in a graphics context.

