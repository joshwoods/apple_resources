

- Core Animation
- CALayer
-  shadowOpacity 

Instance Property

# shadowOpacity

The opacity of the layer’s shadow. Animatable.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var shadowOpacity: Float { get set }
```

## Discussion

The value in this property must be in the range `0.0` (transparent) to `1.0` (opaque). The default value of this property is `0.0`.

## See Also

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

var shadowRadius: CGFloat

The blur radius (in points) used to render the layer’s shadow. Animatable.

var shadowOffset: CGSize

The offset (in points) of the layer’s shadow. Animatable.

