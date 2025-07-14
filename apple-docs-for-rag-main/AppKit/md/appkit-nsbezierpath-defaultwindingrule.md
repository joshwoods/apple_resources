

- AppKit
- NSBezierPath
-  defaultWindingRule 

Type Property

# defaultWindingRule

Returns the default winding rule used to fill all paths.

macOS

``` source
class var defaultWindingRule: NSBezierPath.WindingRule { get set }
```

## Return Value

The current default winding rule or NSNonZeroWindingRule if no default rule has been set. This value may be either NSNonZeroWindingRule or NSEvenOddWindingRule.

## See Also

### Related Documentation

var windingRule: NSBezierPath.WindingRule

The winding rule used to fill the path.

### Configuring Default Path Attributes

class var defaultLineCapStyle: NSBezierPath.LineCapStyle

Returns the default line cap style for all paths.

class var defaultLineJoinStyle: NSBezierPath.LineJoinStyle

Returns the default line join style for all paths.

class var defaultLineWidth: CGFloat

Returns the default line width for the all paths.

class var defaultMiterLimit: CGFloat

Returns the default miter limit for all paths.

class var defaultFlatness: CGFloat

The default flatness value for all paths.

