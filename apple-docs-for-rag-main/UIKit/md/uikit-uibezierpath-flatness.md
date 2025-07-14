

- UIKit
- UIBezierPath
-  flatness 

Instance Property

# flatness

The factor that determines the rendering accuracy for curved path segments.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var flatness: CGFloat { get set }
```

## Discussion

The flatness value measures the largest permissible distance (measured in pixels) between a point on the true curve and a point on the rendered curve. Smaller values result in smoother curves but require more computation time. Larger values result in more jagged curves but are rendered much faster. The default flatness value is `0.6`.

In most cases, you should not change the flatness value. However, you might increase the flatness value temporarily to minimize the amount of time it takes to draw a shape temporarily (such as during scrolling).

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

var usesEvenOddFillRule: Bool

A Boolean value that indicates whether the even-odd winding rule is in use for drawing paths.

func setLineDash(UnsafePointer&lt;CGFloat>?, count: Int, phase: CGFloat)

Sets the line-stroking pattern for the path.

func getLineDash(UnsafeMutablePointer&lt;CGFloat>?, count: UnsafeMutablePointer&lt;Int>?, phase: UnsafeMutablePointer&lt;CGFloat>?)

Retrieves the line-stroking pattern for the path.

