

- UIKit
- UIBezierPath
-  lineCapStyle 

Instance Property

# lineCapStyle

The shape of the endpoints of a stroked path.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var lineCapStyle: CGLineCap { get set }
```

## Discussion

The line cap style is applied to the start and end points of any open subpaths. This property does not affect closed subpaths. The default line cap style is CGLineCap.butt.

## See Also

### Accessing drawing properties

var lineWidth: CGFloat

The line width of the path.

var lineJoinStyle: CGLineJoin

The shape of the joints between connected segments of a stroked path.

var miterLimit: CGFloat

The limiting value that helps avoid spikes at junctions between connected line segments.

var flatness: CGFloat

The factor that determines the rendering accuracy for curved path segments.

var usesEvenOddFillRule: Bool

A Boolean value that indicates whether the even-odd winding rule is in use for drawing paths.

func setLineDash(UnsafePointer&lt;CGFloat>?, count: Int, phase: CGFloat)

Sets the line-stroking pattern for the path.

func getLineDash(UnsafeMutablePointer&lt;CGFloat>?, count: UnsafeMutablePointer&lt;Int>?, phase: UnsafeMutablePointer&lt;CGFloat>?)

Retrieves the line-stroking pattern for the path.

