

- AppKit
- NSBezierPath
-  defaultMiterLimit 

Type Property

# defaultMiterLimit

Returns the default miter limit for all paths.

macOS

``` source
class var defaultMiterLimit: CGFloat { get set }
```

## Return Value

The default miter limit for all paths, or 10.0 if no other value has been set.

## See Also

### Related Documentation

var miterLimit: CGFloat

The limit at which miter joins are converted to bevel joins.

### Configuring Default Path Attributes

class var defaultWindingRule: NSBezierPath.WindingRule

Returns the default winding rule used to fill all paths.

class var defaultLineCapStyle: NSBezierPath.LineCapStyle

Returns the default line cap style for all paths.

class var defaultLineJoinStyle: NSBezierPath.LineJoinStyle

Returns the default line join style for all paths.

class var defaultLineWidth: CGFloat

Returns the default line width for the all paths.

class var defaultFlatness: CGFloat

The default flatness value for all paths.

