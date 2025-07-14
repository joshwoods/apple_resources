

- Core Animation
- CALayer
-  allowsEdgeAntialiasing 

Instance Property

# allowsEdgeAntialiasing

A Boolean indicating whether the layer is allowed to perform edge antialiasing.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var allowsEdgeAntialiasing: Bool { get set }
```

## Discussion

When the value is true, the layer is allowed to antialias its edges, as requested by the value in the layer’s edgeAntialiasingMask property. The default value is read from the boolean `UIViewEdgeAntialiasing` property in the main bundle’s `Info.plist` file. If no value is found, the default value is false.

## See Also

### Related Documentation

var edgeAntialiasingMask: CAEdgeAntialiasingMask

A bitmask defining how the edges of the receiver are rasterized.

### Modifying the Layer’s Appearance

var contentsGravity: CALayerContentsGravity

A constant that specifies how the layer’s contents are positioned or scaled within its bounds.

Contents Gravity Values

The contents gravity constants specify the position of the content object when the layer bounds is larger than the bounds of the content object. They are used by the contentsGravity property.

var opacity: Float

The opacity of the receiver. Animatable.

var isHidden: Bool

A Boolean indicating whether the layer is displayed. Animatable.

var masksToBounds: Bool

A Boolean indicating whether sublayers are clipped to the layer’s bounds. Animatable.

var mask: CALayer?

An optional layer whose alpha channel is used to mask the layer’s content.

var isDoubleSided: Bool

A Boolean indicating whether the layer displays its content when facing away from the viewer. Animatable.

var cornerRadius: CGFloat

The radius to use when drawing rounded corners for the layer’s background. Animatable.

var maskedCorners: CACornerMask

struct CACornerMask

var borderWidth: CGFloat

The width of the layer’s border. Animatable.

var borderColor: CGColor?

The color of the layer’s border. Animatable.

var backgroundColor: CGColor?

The background color of the receiver. Animatable.

var shadowOpacity: Float

The opacity of the layer’s shadow. Animatable.

var shadowRadius: CGFloat

The blur radius (in points) used to render the layer’s shadow. Animatable.

