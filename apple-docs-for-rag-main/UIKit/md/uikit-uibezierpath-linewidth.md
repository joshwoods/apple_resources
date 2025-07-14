

- UIKit
- UIBezierPath
-  lineWidth 

Instance Property

# lineWidth

The line width of the path.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var lineWidth: CGFloat { get set }
```

## Discussion

The line width defines the thickness of the receiver’s stroked path. A width of 0 is interpreted as the thinnest line that can be rendered on a particular device. The actual rendered line width may vary from the specified width by as much as 2 device pixels, depending on the position of the line with respect to the pixel grid and the current anti-aliasing settings. The width of the line may also be affected by scaling factors specified in the current transformation matrix of the active graphics context.

The default line width is 1.0.

## See Also

### Accessing drawing properties

var lineCapStyle: CGLineCap

The shape of the endpoints of a stroked path.

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

