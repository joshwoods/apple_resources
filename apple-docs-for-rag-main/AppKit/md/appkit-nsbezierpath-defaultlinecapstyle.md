

- AppKit
- NSBezierPath
-  defaultLineCapStyle 

Type Property

# defaultLineCapStyle

Returns the default line cap style for all paths.

macOS

``` source
class var defaultLineCapStyle: NSBezierPath.LineCapStyle { get set }
```

## Return Value

The default line cap style or `NSButtLineCapStyle` if no other style has been set. For a list of values, see Constants.

## Discussion

The default line cap style can be overridden for individual paths by setting a custom style for that path using the NSBezierPath method.

## See Also

### Related Documentation

var lineCapStyle: NSBezierPath.LineCapStyle

The line cap style for the path.

### Configuring Default Path Attributes

class var defaultWindingRule: NSBezierPath.WindingRule

Returns the default winding rule used to fill all paths.

class var defaultLineJoinStyle: NSBezierPath.LineJoinStyle

Returns the default line join style for all paths.

class var defaultLineWidth: CGFloat

Returns the default line width for the all paths.

class var defaultMiterLimit: CGFloat

Returns the default miter limit for all paths.

class var defaultFlatness: CGFloat

The default flatness value for all paths.

