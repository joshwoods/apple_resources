

- AppKit
- NSBezierPath
-  getLineDash(\_:count:phase:) 

Instance Method

# getLineDash(\_:count:phase:)

Returns the line-stroking pattern for the receiver.

macOS

``` source
func getLineDash(
    _ pattern: UnsafeMutablePointer?,
    count: UnsafeMutablePointer?,
    phase: UnsafeMutablePointer?
)
```

## Parameters 

`pattern`  

On input, a C-style array of floating point values, or `nil` if you do not want the pattern values. On output, this array contains the lengths (measured in points) of the line segments and gaps in the pattern. The values in the array alternate, starting with the first line segment length, followed by the first gap length, followed by the second line segment length, and so on.

`count`  

On input, a pointer to an integer or `nil` if you do not want the number of pattern entries. On output, the number of entries written to `pattern`.

`phase`  

On input, a pointer to a floating point value or `nil` if you do not want the phase. On output, this value contains the offset at which to start drawing the pattern, measured in points along the dashed-line pattern. For example, a phase of 6 in the pattern 5-2-3-2 would cause drawing to begin in the middle of the first gap.

## Discussion

The array in the `pattern` parameter must be large enough to hold all of the returned values in the pattern. If you are not sure how many values there might be, you can call this method twice. The first time you call it, do not pass a value for `pattern` but use the returned value in `count` to allocate an array of floating-point numbers that you can then pass in the second time.

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

func setLineDash(UnsafePointer&lt;CGFloat>?, count: Int, phase: CGFloat)

Sets the line-stroking pattern for the path.

