

- Core Animation
- CALayer
-  minificationFilterBias 

Instance Property

# minificationFilterBias

The bias factor used by the minification filter to determine the levels of detail.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var minificationFilterBias: Float { get set }
```

## Discussion

This value is used by the minificationFilter when it is set to trilinear.

The default value of this property is `0.0`.

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

var magnificationFilter: CALayerContentsFilter

The filter used when increasing the size of the content.

