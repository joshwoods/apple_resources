

- Core Animation
-  CATiledLayer 

Class

# CATiledLayer

A layer that provides a way to asynchronously provide tiles of the layer’s content, potentially cached at multiple levels of detail.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
class CATiledLayer
```

## Overview

As more data is required by the renderer, the layer’s draw(in:) method is called on one or more background threads to supply the drawing operations to fill in one tile of data. The clip bounds and current transformation matrix (CTM) of the drawing context can be used to determine the bounds and resolution of the tile being requested.

Regions of the layer may be invalidated using the setNeedsDisplay(_:) method however the update will be asynchronous. While the next display update will most likely not contain the updated content, a future update will.

Important

Do not attempt to directly modify the contents property of a CATiledLayer object. Doing so disables the ability of a tiled layer to asynchronously provide tiled content, effectively turning the layer into a regular CALayer object.

## Topics

### Visual Fade

class func fadeDuration() -> CFTimeInterval

The time, in seconds, that newly added images take to “fade-in” to the rendered representation of the tiled layer.

### Levels of detail

var levelsOfDetail: Int

The number of levels of detail maintained by this layer.

var levelsOfDetailBias: Int

The number of magnified levels of detail for this layer.

### Layer tile size

var tileSize: CGSize

The maximum size of each tile used to create the layer’s content.

## Relationships

### Inherits From

- CALayer

### Conforms To

- CAMediaTiming
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Advanced Layer Options

class CAScrollLayer

A layer that displays scrollable content larger than its own bounds.

class CATransformLayer

Objects used to create true 3D layer hierarchies, rather than the flattened hierarchy rendering model used by other layer types.

class CAReplicatorLayer

A layer that creates a specified number of sublayer copies with varying geometric, temporal, and color transformations.

