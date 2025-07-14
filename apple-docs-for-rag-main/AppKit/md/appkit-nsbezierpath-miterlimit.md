

- AppKit
- NSBezierPath
-  miterLimit 

Instance Property

# miterLimit

The limit at which miter joins are converted to bevel joins.

macOS

``` source
var miterLimit: CGFloat { get set }
```

## Discussion

The miter limit helps you avoid spikes at the junction of two line segments connected by a miter join (NSMiterLineJoinStyle). If the ratio of the miter length—the diagonal length of the miter join—to the line thickness exceeds the miter limit, the joint is converted to a bevel join.

The default value of this property is the value returned by the defaultMiterLimit method.

## See Also

### Related Documentation

class var defaultMiterLimit: CGFloat

Returns the default miter limit for all paths.

### Accessing a Path’s Attributes

var windingRule: NSBezierPath.WindingRule

The winding rule used to fill the path.

var lineCapStyle: NSBezierPath.LineCapStyle

The line cap style for the path.

var lineJoinStyle: NSBezierPath.LineJoinStyle

The line join style for the path.

var lineWidth: CGFloat

The width of stroked path lines.

var flatness: CGFloat

The accuracy with which curves are rendered.

func getLineDash(UnsafeMutablePointer&lt;CGFloat>?, count: UnsafeMutablePointer&lt;Int>?, phase: UnsafeMutablePointer&lt;CGFloat>?)

Returns the line-stroking pattern for the receiver.

func setLineDash(UnsafePointer&lt;CGFloat>?, count: Int, phase: CGFloat)

Sets the line-stroking pattern for the path.

