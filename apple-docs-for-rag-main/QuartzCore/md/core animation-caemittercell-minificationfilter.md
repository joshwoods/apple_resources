

- Core Animation
- CAEmitterCell
-  minificationFilter 

Instance Property

# minificationFilter

The filter used when reducing the size of the content.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
var minificationFilter: String { get set }
```

## Discussion

The possible values for this property are listed in Scaling Filters. The default value is linear.

## See Also

### Setting Emitter Cell Visual Attributes

var isEnabled: Bool

A Boolean value indicating whether or not cells from this emitter are rendered.

var color: CGColor?

The color of each emitted object. Animatable.

var redRange: Float

The amount by which the red color component of the cell can vary. Animatable.

var greenRange: Float

The amount by which the green color component of the cell can vary. Animatable.

var blueRange: Float

The amount by which the blue color component of the cell can vary. Animatable.

var alphaRange: Float

The amount by which the alpha component of the cell can vary. Animatable.

var redSpeed: Float

The speed, in seconds, at which the red color component changes over the lifetime of the cell. Animatable.

var greenSpeed: Float

The speed, in seconds, at which the green color component changes over the lifetime of the cell. Animatable.

var blueSpeed: Float

The speed, in seconds, at which the blue color component changes over the lifetime of the cell. Animatable.

var alphaSpeed: Float

The speed, in seconds, at which the alpha component changes over the lifetime of the cell. Animatable.

var magnificationFilter: String

The filter used when increasing the size of the content.

var minificationFilterBias: Float

The bias factor used by the minification filter to determine the levels of detail.

var scale: CGFloat

Specifies the scale factor applied to the cell. Animatable.

var scaleRange: CGFloat

Specifies the range over which the scale value can vary. Animatable.

var contentsScale: CGFloat

The scale factor of the cell contents.

