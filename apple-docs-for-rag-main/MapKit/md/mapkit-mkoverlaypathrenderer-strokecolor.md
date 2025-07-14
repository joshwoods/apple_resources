

- MapKit
- MKOverlayPathRenderer
-  strokeColor 

Instance Property

# strokeColor

The stroke color to use for the path.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
var strokeColor: UIColor? { get set }
```

**macOS**

``` source
var strokeColor: NSColor? { get set }
```

## See Also

### Accessing the drawing attributes

var fillColor: UIColor?

The fill color to use for the path.

var lineWidth: CGFloat

The stroke width to use for the path.

var lineJoin: CGLineJoin

The line join style to apply to the corners of the path.

var lineCap: CGLineCap

The line cap style to apply to the open ends of the path.

var miterLimit: CGFloat

The limiting value that helps avoid spikes at junctions between connected line segments.

var lineDashPhase: CGFloat

The offset (in points) at which to start drawing the dash pattern.

var lineDashPattern: [NSNumber]?

An array of numbers specifying the dash pattern to use for the path.

