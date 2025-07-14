

- PencilKit
-  PKStrokeReference 

Class

# PKStrokeReference

A class that represents the paths, boundaries and other properties of a stroke drawn on a canvas.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
class PKStrokeReference
```

## Topics

### Creating a stroke object

init(ink: PKInk, strokePath: PKStrokePath, transform: CGAffineTransform, mask: UIBezierPath?)

Creates a stroke with the line properties, path, transform, and mask that you specify.

init(ink: PKInk, strokePath: PKStrokePath, transform: CGAffineTransform, mask: UIBezierPath?, randomSeed: UInt32)

Creates a stroke with the line properties, path, transform, mask, and random seed that you specify.

### Getting the stroke properties

var ink: PKInk

The line properties used to render this stroke.

var mask: UIBezierPath?

The pretransform mask used to clip the rendering of the stroke.

var maskedPathRanges: [__PKFloatRange]

The range of points in the stroke path reference that intersect the stroke’s mask.

var path: PKStrokePath

The B-spline path that describes this stroke.

var renderBounds: CGRect

The bounds of the rendered stroke, including the width and line properties of the stroke after applying the transform.

var transform: CGAffineTransform

The affine transform of the stroke after rendering.

var randomSeed: UInt32

An unsigned 32-bit integer to use as a random seed for drawing strokes that use randomized effects.

### Supporting backward compatibility

var requiredContentVersion: PKContentVersion

The version of PencilKit necessary to use the stroke.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

