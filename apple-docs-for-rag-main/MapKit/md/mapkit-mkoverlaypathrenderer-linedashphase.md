

- MapKit
- MKOverlayPathRenderer
-  lineDashPhase 

Instance Property

# lineDashPhase

The offset (in points) at which to start drawing the dash pattern.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var lineDashPhase: CGFloat { get set }
```

## Discussion

Use this property to start drawing a dashed line partway through a segment or gap. For example, a phase value of `6` for the pattern 5-2-3-2 would cause drawing to begin in the middle of the first gap.

The default value of this property is `0`.

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

var lineCap: CGLineCap

The line cap style to apply to the open ends of the path.

var miterLimit: CGFloat

The limiting value that helps avoid spikes at junctions between connected line segments.

var lineDashPattern: [NSNumber]?

An array of numbers specifying the dash pattern to use for the path.

