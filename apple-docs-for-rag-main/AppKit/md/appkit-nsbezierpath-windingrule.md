

- AppKit
- NSBezierPath
-  windingRule 

Instance Property

# windingRule

The winding rule used to fill the path.

macOS

``` source
var windingRule: NSBezierPath.WindingRule { get set }
```

## Discussion

This value may be either NSNonZeroWindingRule or NSEvenOddWindingRule. This value overrides the default value returned by the defaultWindingRule method.

For more information on how winding rules affect the appearance of filled paths, see Cocoa Drawing Guide.

## See Also

### Related Documentation

func fill()

Paints the region enclosed by the path.

class var defaultWindingRule: NSBezierPath.WindingRule

Returns the default winding rule used to fill all paths.

### Accessing a Path’s Attributes

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

func setLineDash(UnsafePointer&lt;CGFloat>?, count: Int, phase: CGFloat)

Sets the line-stroking pattern for the path.

