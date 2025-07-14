

- AppKit
- NSBezierPath
-  defaultLineWidth 

Type Property

# defaultLineWidth

Returns the default line width for the all paths.

macOS

``` source
class var defaultLineWidth: CGFloat { get set }
```

## Return Value

The default line width, measured in points in the user coordinate space, or 1.0 if no other value has been set.

## See Also

### Related Documentation

var lineWidth: CGFloat

The width of stroked path lines.

### Configuring Default Path Attributes

class var defaultWindingRule: NSBezierPath.WindingRule

Returns the default winding rule used to fill all paths.

class var defaultLineCapStyle: NSBezierPath.LineCapStyle

Returns the default line cap style for all paths.

class var defaultLineJoinStyle: NSBezierPath.LineJoinStyle

Returns the default line join style for all paths.

class var defaultMiterLimit: CGFloat

Returns the default miter limit for all paths.

class var defaultFlatness: CGFloat

The default flatness value for all paths.

