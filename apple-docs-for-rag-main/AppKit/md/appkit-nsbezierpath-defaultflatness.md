

- AppKit
- NSBezierPath
-  defaultFlatness 

Type Property

# defaultFlatness

The default flatness value for all paths.

macOS

``` source
class var defaultFlatness: CGFloat { get set }
```

## Return Value

The default value for determining the smoothness of curved paths, or 0.6 if no other value has been set.

## See Also

### Related Documentation

var flatness: CGFloat

The accuracy with which curves are rendered.

### Configuring Default Path Attributes

class var defaultWindingRule: NSBezierPath.WindingRule

Returns the default winding rule used to fill all paths.

class var defaultLineCapStyle: NSBezierPath.LineCapStyle

Returns the default line cap style for all paths.

class var defaultLineJoinStyle: NSBezierPath.LineJoinStyle

Returns the default line join style for all paths.

class var defaultLineWidth: CGFloat

Returns the default line width for the all paths.

class var defaultMiterLimit: CGFloat

Returns the default miter limit for all paths.

