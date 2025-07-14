

- AppKit
- NSBezierPath
-  lineCapStyle 

Instance Property

# lineCapStyle

The line cap style for the path.

macOS

``` source
var lineCapStyle: NSBezierPath.LineCapStyle { get set }
```

## Discussion

The line cap style specifies the shape of the endpoints on an open path when stroked. The default value of this property is the value returned by the defaultLineCapStyle method.

## See Also

### Related Documentation

class var defaultLineCapStyle: NSBezierPath.LineCapStyle

Returns the default line cap style for all paths.

enum LineCapStyle

Constants that specify the shape of endpoints for an open path when it is stroked.

### Accessing a Path’s Attributes

var windingRule: NSBezierPath.WindingRule

The winding rule used to fill the path.

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

func setLineDash(UnsafePointer&lt;CGFloat>?, count: Int, phase: CGFloat)

Sets the line-stroking pattern for the path.

