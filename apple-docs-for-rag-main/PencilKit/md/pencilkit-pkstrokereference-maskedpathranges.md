

- PencilKit
- PKStrokeReference
-  maskedPathRanges 

Instance Property

# maskedPathRanges

The range of points in the stroke path reference that intersect the stroke’s mask.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
var maskedPathRanges: [__PKFloatRange] { get }
```

## See Also

### Getting the stroke properties

var ink: PKInk

The line properties used to render this stroke.

var mask: UIBezierPath?

The pretransform mask used to clip the rendering of the stroke.

var path: PKStrokePath

The B-spline path that describes this stroke.

var renderBounds: CGRect

The bounds of the rendered stroke, including the width and line properties of the stroke after applying the transform.

var transform: CGAffineTransform

The affine transform of the stroke after rendering.

var randomSeed: UInt32

An unsigned 32-bit integer to use as a random seed for drawing strokes that use randomized effects.

