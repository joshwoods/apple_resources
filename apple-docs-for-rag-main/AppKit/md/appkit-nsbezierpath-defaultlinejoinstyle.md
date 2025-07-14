

- AppKit
- NSBezierPath
-  defaultLineJoinStyle 

Type Property

# defaultLineJoinStyle

Returns the default line join style for all paths.

macOS

``` source
class var defaultLineJoinStyle: NSBezierPath.LineJoinStyle { get set }
```

## Return Value

The default line join style or `NSMiterLineJoinStyle` if no other value has been set. For a list of values, see Constants.

## See Also

### Related Documentation

var lineJoinStyle: NSBezierPath.LineJoinStyle

The line join style for the path.

### Configuring Default Path Attributes

class var defaultWindingRule: NSBezierPath.WindingRule

Returns the default winding rule used to fill all paths.

class var defaultLineCapStyle: NSBezierPath.LineCapStyle

Returns the default line cap style for all paths.

class var defaultLineWidth: CGFloat

Returns the default line width for the all paths.

class var defaultMiterLimit: CGFloat

Returns the default miter limit for all paths.

class var defaultFlatness: CGFloat

The default flatness value for all paths.

