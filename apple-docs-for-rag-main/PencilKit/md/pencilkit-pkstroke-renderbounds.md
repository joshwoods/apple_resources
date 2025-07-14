

- PencilKit
- PKStroke
-  renderBounds 

Instance Property

# renderBounds

The bounds of the rendered stroke, including the width and line properties of the stroke after applying the transform.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
var renderBounds: CGRect { get }
```

## See Also

### Getting the stroke properties

var ink: PKInk

The Ink, which is a combination of a tool used to render this stroke.

var mask: UIBezierPath?

The pretransform mask used to clip the rendering of the stroke.

var mask: NSBezierPath?

The pretransform mask used to clip the rendering of the stroke.

var maskedPathRanges: [ClosedRange&lt;CGFloat>]

The range of points in the stroke path reference that intersect the stroke’s mask.

var path: PKStrokePath

The B-spline path that describes this stroke.

var transform: CGAffineTransform

The affine transform of the stroke after rendering.

var randomSeed: UInt32

