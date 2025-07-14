

- UIKit
- UIBezierPath
-  usesEvenOddFillRule 

Instance Property

# usesEvenOddFillRule

A Boolean value that indicates whether the even-odd winding rule is in use for drawing paths.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var usesEvenOddFillRule: Bool { get set }
```

## Discussion

If true, the path is filled using the even-odd rule. If false, it is filled using the non-zero rule. Both rules are algorithms to determine which areas of a path to fill with the current fill color. A ray is drawn from a point inside a given region to a point anywhere outside the path’s bounds. The total number of crossed path lines (including implicit path lines) and the direction of each path line are then interpreted as follows:

- For the even-odd rule, if the total number of path crossings is odd, the point is considered to be inside the path and the corresponding region is filled. If the number of crossings is even, the point is considered to be outside the path and the region is not filled.

- For the non-zero rule, the crossing of a left-to-right path counts as +1 and the crossing of a right-to-left path counts as -1. If the sum of the crossings is nonzero, the point is considered to be inside the path and the corresponding region is filled. If the sum is 0, the point is outside the path and the region is not filled.

The default value of this property is false. For more information about winding rules and how they are applied to subpaths, see Quartz 2D Programming Guide.

## See Also

### Accessing drawing properties

var lineWidth: CGFloat

The line width of the path.

var lineCapStyle: CGLineCap

The shape of the endpoints of a stroked path.

var lineJoinStyle: CGLineJoin

The shape of the joints between connected segments of a stroked path.

var miterLimit: CGFloat

The limiting value that helps avoid spikes at junctions between connected line segments.

var flatness: CGFloat

The factor that determines the rendering accuracy for curved path segments.

func setLineDash(UnsafePointer&lt;CGFloat>?, count: Int, phase: CGFloat)

Sets the line-stroking pattern for the path.

func getLineDash(UnsafeMutablePointer&lt;CGFloat>?, count: UnsafeMutablePointer&lt;Int>?, phase: UnsafeMutablePointer&lt;CGFloat>?)

Retrieves the line-stroking pattern for the path.

