

- AppKit
- NSBezierPath
-  lineJoinStyle 

Instance Property

# lineJoinStyle

The line join style for the path.

macOS

``` source
var lineJoinStyle: NSBezierPath.LineJoinStyle { get set }
```

## Discussion

The line join style specifies the shape of the joints between connected segments of a stroked path. The default value of this property is the value returned by the defaultLineJoinStyle method.

## See Also

### Related Documentation

class var defaultLineJoinStyle: NSBezierPath.LineJoinStyle

Returns the default line join style for all paths.

enum LineJoinStyle

Constants that specify the shape of the joins between connected segments of a stroked path.

### Accessing a Path’s Attributes

var windingRule: NSBezierPath.WindingRule

The winding rule used to fill the path.

var lineCapStyle: NSBezierPath.LineCapStyle

The line cap style for the path.

var lineWidth: CGFloat

The width of stroked path lines.

var miterLimit: CGFloat

The limit at which miter joins are converted to bevel joins.

var flatness: CGFloat

The accuracy with which curves are rendered.

func getLineDash(UnsafeMutablePointer&lt;CGFloat>?, count: UnsafeMutablePointer&lt;Int>?, phase: UnsafeMutablePointer&lt;CGFloat>?)

Returns the line-stroking pattern for the receiver.

func setLineDash(UnsafePointer&lt;CGFloat>?, count: Int, phase: CGFloat)

Sets the line-stroking pattern for the path.

