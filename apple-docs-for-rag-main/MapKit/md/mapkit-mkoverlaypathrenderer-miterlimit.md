

- MapKit
- MKOverlayPathRenderer
-  miterLimit 

Instance Property

# miterLimit

The limiting value that helps avoid spikes at junctions between connected line segments.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var miterLimit: CGFloat { get set }
```

## Discussion

The miter limit helps you avoid spikes in paths that use the CGLineJoin.miter join style. If the ratio of the miter length to the line thickness — the diagonal length of the miter join — exceeds the miter limit, the renderer converts the joint to a bevel join. The default miter limit is `10`, which results in the conversion of miters with an angle at the joint of less than `11` degrees.

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

var lineDashPhase: CGFloat

The offset (in points) at which to start drawing the dash pattern.

var lineDashPattern: [NSNumber]?

An array of numbers specifying the dash pattern to use for the path.

