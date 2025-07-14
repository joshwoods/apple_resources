

- Core Animation
- CALayer
-  minificationFilter 

Instance Property

# minificationFilter

The filter used when reducing the size of the content.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var minificationFilter: CALayerContentsFilter { get set }
```

## Discussion

The possible values for this property are listed in Scaling Filters.

The default value of this property is linear.

## See Also

### Layer Filters

var filters: [Any]?

An array of Core Image filters to apply to the contents of the layer and its sublayers. Animatable.

var compositingFilter: Any?

A CoreImage filter used to composite the layer and the content behind it. Animatable.

var backgroundFilters: [Any]?

An array of Core Image filters to apply to the content immediately behind the layer. Animatable.

var minificationFilterBias: Float

The bias factor used by the minification filter to determine the levels of detail.

var magnificationFilter: CALayerContentsFilter

The filter used when increasing the size of the content.

