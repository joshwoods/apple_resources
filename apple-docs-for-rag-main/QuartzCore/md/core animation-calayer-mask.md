

- Core Animation
- CALayer
-  mask 

Instance Property

# mask

An optional layer whose alpha channel is used to mask the layer’s content.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var mask: CALayer? { get set }
```

## Discussion

The layer’s alpha channel determines how much of the layer’s content and background shows through. Fully or partially opaque pixels allow the underlying content to show through, but fully transparent pixels block that content.

The default value of this property is `nil`. When configuring a mask, remember to set the size and position of the mask layer to ensure it is aligned properly with the layer it masks.

### Special Considerations

The layer you assign to this property must not have a superlayer. If it does, the behavior is undefined.

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

var shadowOffset: CGSize

The offset (in points) of the layer’s shadow. Animatable.

