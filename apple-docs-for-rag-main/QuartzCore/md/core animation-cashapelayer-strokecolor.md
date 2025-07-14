

- Core Animation
- CAShapeLayer
-  strokeColor 

Instance Property

# strokeColor

The color used to stroke the shape’s path. Animatable.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
var strokeColor: CGColor? { get set }
```

## Discussion

Setting `strokeColor` to `nil` results in no stroke being rendered.

Default is `nil`.

## See Also

### Accessing Shape Style Properties

var fillColor: CGColor?

The color used to fill the shape’s path. Animatable.

var fillRule: CAShapeLayerFillRule

The fill rule used when filling the shape’s path.

var lineCap: CAShapeLayerLineCap

Specifies the line cap style for the shape’s path.

var lineDashPattern: [NSNumber]?

The dash pattern applied to the shape’s path when stroked.

var lineDashPhase: CGFloat

The dash phase applied to the shape’s path when stroked. Animatable.

var lineJoin: CAShapeLayerLineJoin

Specifies the line join style for the shape’s path.

var lineWidth: CGFloat

Specifies the line width of the shape’s path. Animatable.

var miterLimit: CGFloat

The miter limit used when stroking the shape’s path. Animatable.

var strokeStart: CGFloat

The relative location at which to begin stroking the path. Animatable.

var strokeEnd: CGFloat

The relative location at which to stop stroking the path. Animatable.

