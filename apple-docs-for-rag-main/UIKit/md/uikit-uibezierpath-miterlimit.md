

- UIKit
- UIBezierPath
-  miterLimit 

Instance Property

# miterLimit

The limiting value that helps avoid spikes at junctions between connected line segments.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var miterLimit: CGFloat { get set }
```

## Discussion

The miter limit helps you avoid spikes in paths that use the CGLineJoin.miter join style. If the ratio of the miter length—that is, the diagonal length of the miter join—to the line thickness exceeds the miter limit, the joint is converted to a bevel join. The default miter limit is 10, which results in the conversion of miters whose angle at the joint is less than 11 degrees.

## See Also

### Accessing drawing properties

var lineWidth: CGFloat

The line width of the path.

var lineCapStyle: CGLineCap

The shape of the endpoints of a stroked path.

var lineJoinStyle: CGLineJoin

The shape of the joints between connected segments of a stroked path.

var flatness: CGFloat

The factor that determines the rendering accuracy for curved path segments.

var usesEvenOddFillRule: Bool

A Boolean value that indicates whether the even-odd winding rule is in use for drawing paths.

func setLineDash(UnsafePointer&lt;CGFloat>?, count: Int, phase: CGFloat)

Sets the line-stroking pattern for the path.

func getLineDash(UnsafeMutablePointer&lt;CGFloat>?, count: UnsafeMutablePointer&lt;Int>?, phase: UnsafeMutablePointer&lt;CGFloat>?)

Retrieves the line-stroking pattern for the path.

