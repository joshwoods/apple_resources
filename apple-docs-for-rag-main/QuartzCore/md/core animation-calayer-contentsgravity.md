

- Core Animation
- CALayer
-  contentsGravity 

Instance Property

# contentsGravity

A constant that specifies how the layer’s contents are positioned or scaled within its bounds.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var contentsGravity: CALayerContentsGravity { get set }
```

## Discussion

The possible values for this property are listed in Contents Gravity Values.

The default value of this property is resize.

Important

The naming of contents gravity constants is based on the direction of the vertical axis. If you are using gravity constants with a vertical component, e.g. top, you should also check the layer’s contentsAreFlipped(). When this is true, top aligns contents to the bottom of the layer and bottom aligns content to the top of the layer.

The default coordinate system for views in macOS and iOS differ in the orientation of the vertical axis: in macOS, the default coordinate system has its origin at the lower left of the drawing area and positive values extend up from it, and in iOS the default coordinate system has its origin at the upper left of the drawing area and positive values extend down from it.

For more information, see Coordinate system.

Figure 1 shows four examples of the effect of setting different values for a layer’s contentsGravity property.

1.  Contents gravity is resize - the default

2.  Contents gravity is center

3.  Contents gravity is contentsAreFlipped() `?` top : bottom

4.  Contents gravity is contentsAreFlipped() `?` bottomLeft : topLeft

## See Also

### Modifying the Layer’s Appearance

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

var shadowOffset: CGSize

The offset (in points) of the layer’s shadow. Animatable.

