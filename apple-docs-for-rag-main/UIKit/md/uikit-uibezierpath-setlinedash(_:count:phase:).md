

- UIKit
- UIBezierPath
-  setLineDash(\_:count:phase:) 

Instance Method

# setLineDash(\_:count:phase:)

Sets the line-stroking pattern for the path.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func setLineDash(
    _ pattern: UnsafePointer?,
    count: Int,
    phase: CGFloat
)
```

## Parameters 

`pattern`  

A C-style array of floating point values that contains the lengths (measured in points) of the line segments and gaps in the pattern. The values in the array alternate, starting with the first line segment length, followed by the first gap length, followed by the second line segment length, and so on.

`count`  

The number of values in `pattern`.

`phase`  

The offset at which to start drawing the pattern, measured in points along the dashed-line pattern. For example, a phase value of `6` for the pattern 5-2-3-2 would cause drawing to begin in the middle of the first gap.

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

var usesEvenOddFillRule: Bool

A Boolean value that indicates whether the even-odd winding rule is in use for drawing paths.

func getLineDash(UnsafeMutablePointer&lt;CGFloat>?, count: UnsafeMutablePointer&lt;Int>?, phase: UnsafeMutablePointer&lt;CGFloat>?)

Retrieves the line-stroking pattern for the path.

