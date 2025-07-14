

- AppKit
- NSBezierPath
-  flatness 

Instance Property

# flatness

The accuracy with which curves are rendered.

macOS

``` source
var flatness: CGFloat { get set }
```

## Discussion

The flatness value specifies the accuracy (or smoothness) with which curves are rendered. It is also the maximum error tolerance (measured in pixels) for rendering curves, where smaller numbers give smoother curves at the expense of more computation. The exact interpretation may vary slightly on different rendering devices.

The default value of this property is the value returned by the defaultFlatness method.

## See Also

### Related Documentation

class var defaultFlatness: CGFloat

The default flatness value for all paths.

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

func getLineDash(UnsafeMutablePointer&lt;CGFloat>?, count: UnsafeMutablePointer&lt;Int>?, phase: UnsafeMutablePointer&lt;CGFloat>?)

Returns the line-stroking pattern for the receiver.

func setLineDash(UnsafePointer&lt;CGFloat>?, count: Int, phase: CGFloat)

Sets the line-stroking pattern for the path.

