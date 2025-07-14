

- Core Animation
- CALayer
-  Contents Gravity Values 

API Collection

# Contents Gravity Values

The contents gravity constants specify the position of the content object when the layer bounds is larger than the bounds of the content object. They are used by the contentsGravity property.

## Topics

### Constants

static let center: CALayerContentsGravity

The content is horizontally and vertically centered in the bounds rectangle.

static let top: CALayerContentsGravity

The content is horizontally centered at the top-edge of the bounds rectangle.

static let bottom: CALayerContentsGravity

The content is horizontally centered at the bottom-edge of the bounds rectangle.

static let left: CALayerContentsGravity

The content is vertically centered at the left-edge of the bounds rectangle.

static let right: CALayerContentsGravity

The content is vertically centered at the right-edge of the bounds rectangle.

static let topLeft: CALayerContentsGravity

The content is positioned in the top-left corner of the bounds rectangle.

static let topRight: CALayerContentsGravity

The content is positioned in the top-right corner of the bounds rectangle.

static let bottomLeft: CALayerContentsGravity

The content is positioned in the bottom-left corner of the bounds rectangle.

static let bottomRight: CALayerContentsGravity

The content is positioned in the bottom-right corner of the bounds rectangle.

static let resize: CALayerContentsGravity

The content is resized to fit the entire bounds rectangle.

static let resizeAspect: CALayerContentsGravity

The content is resized to fit the bounds rectangle, preserving the aspect of the content. If the content does not completely fill the bounds rectangle, the content is centered in the partial axis.

static let resizeAspectFill: CALayerContentsGravity

The content is resized to completely fill the bounds rectangle, while still preserving the aspect of the content. The content is centered in the axis it exceeds.

## See Also

### Modifying the Layer’s Appearance

var contentsGravity: CALayerContentsGravity

A constant that specifies how the layer’s contents are positioned or scaled within its bounds.

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

