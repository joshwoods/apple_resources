

- AppKit
- NSBezierPath
-  setLineDash(\_:count:phase:) 

Instance Method

# setLineDash(\_:count:phase:)

Sets the line-stroking pattern for the path.

macOS

``` source
func setLineDash(
    _ pattern: UnsafePointer?,
    count: Int,
    phase: CGFloat
)
```

## Parameters 

`pattern`  

A C-style array of floating point values that contains the lengths (measured in points) of the line segments and gaps in the pattern. The values in the array alternate, starting with the first line segment length, followed by the first gap length, followed by the second line segment length, and so on

`count`  

The number of values in `pattern`.

`phase`  

The offset at which to start drawing the pattern, measured in points along the dashed-line pattern. For example, a phase of 6 in the pattern 5-2-3-2 would cause drawing to begin in the middle of the first gap

## Discussion

For example, to produce a supermarket coupon type of dashed line:

```
array[0] = 5.0; //segment painted with stroke color
array[1] = 2.0; //segment not painted with a color

[path setLineDash: array count: 2 phase: 0.0];
```

In the above example, if you set `phase` to 6.0, the line dash would begin exactly six units into `pattern`, which would start the pattern in the middle of the first gap.

## See Also

### Accessing a Path’s Attributes

var windingRule: NSBezierPath.WindingRule

The winding rule used to fill the path.

var lineCapStyle: NSBezierPath.LineCapStyle

The line cap style for the path.

var lineJoinStyle: NSBezierPath.LineJoinStyle

The line join style for the path.

var lineWidth: CGFloat

The width of stroked path lines.

var miterLimit: CGFloat

The limit at which miter joins are converted to bevel joins.

var flatness: CGFloat

The accuracy with which curves are rendered.

func getLineDash(UnsafeMutablePointer&lt;CGFloat>?, count: UnsafeMutablePointer&lt;Int>?, phase: UnsafeMutablePointer&lt;CGFloat>?)

Returns the line-stroking pattern for the receiver.

