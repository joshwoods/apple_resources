

- PencilKit
- PKStrokeReference
-  randomSeed 

Instance Property

# randomSeed

An unsigned 32-bit integer to use as a random seed for drawing strokes that use randomized effects.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var randomSeed: UInt32 { get }
```

## See Also

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

