

- MapKit
- MKOverlayPathRenderer
-  lineJoin 

Instance Property

# lineJoin

The line join style to apply to the corners of the path.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var lineJoin: CGLineJoin { get set }
```

## Discussion

The default line join style is CGLineJoin.round.

## See Also

### Accessing the drawing attributes

var fillColor: UIColor?

The fill color to use for the path.

var strokeColor: UIColor?

The stroke color to use for the path.

var lineWidth: CGFloat

The stroke width to use for the path.

var lineCap: CGLineCap

The line cap style to apply to the open ends of the path.

var miterLimit: CGFloat

The limiting value that helps avoid spikes at junctions between connected line segments.

var lineDashPhase: CGFloat

The offset (in points) at which to start drawing the dash pattern.

var lineDashPattern: [NSNumber]?

An array of numbers specifying the dash pattern to use for the path.

