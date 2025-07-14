

- Core Animation
- CALayer
-  magnificationFilter 

Instance Property

# magnificationFilter

The filter used when increasing the size of the content.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var magnificationFilter: CALayerContentsFilter { get set }
```

## Discussion

The possible values for this property are listed in Scaling Filters.

The default value of this property is linear.

Figure 1 shows the difference between linear and nearest filtering when a 10 x 10 point image of a circle is magnified by a scale of 10.

The circle on the left uses linear and the circle on the right uses nearest.

## See Also

### Layer Filters

var filters: [Any]?

An array of Core Image filters to apply to the contents of the layer and its sublayers. Animatable.

var compositingFilter: Any?

A CoreImage filter used to composite the layer and the content behind it. Animatable.

var backgroundFilters: [Any]?

An array of Core Image filters to apply to the content immediately behind the layer. Animatable.

var minificationFilter: CALayerContentsFilter

The filter used when reducing the size of the content.

var minificationFilterBias: Float

The bias factor used by the minification filter to determine the levels of detail.

