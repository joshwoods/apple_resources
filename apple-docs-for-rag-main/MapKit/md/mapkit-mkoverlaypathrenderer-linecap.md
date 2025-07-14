

- MapKit
- MKOverlayPathRenderer
-  lineCap 

Instance Property

# lineCap

The line cap style to apply to the open ends of the path.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var lineCap: CGLineCap { get set }
```

## Discussion

The line cap style applies to the start and end points of any open subpaths. This property doesn’t affect closed subpaths. The default line cap style is CGLineCap.round.

## See Also

### Accessing the drawing attributes

var fillColor: UIColor?

The fill color to use for the path.

var strokeColor: UIColor?

The stroke color to use for the path.

var lineWidth: CGFloat

The stroke width to use for the path.

var lineJoin: CGLineJoin

The line join style to apply to the corners of the path.

var miterLimit: CGFloat

The limiting value that helps avoid spikes at junctions between connected line segments.

var lineDashPhase: CGFloat

The offset (in points) at which to start drawing the dash pattern.

var lineDashPattern: [NSNumber]?

An array of numbers specifying the dash pattern to use for the path.

