

- Core Animation
- CAGradientLayer
-  endPoint 

Instance Property

# endPoint

The end point of the gradient when drawn in the layer’s coordinate space. Animatable.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
var endPoint: CGPoint { get set }
```

## Discussion

The end point corresponds to the last stop of the gradient. The point is defined in the unit coordinate space and is then mapped to the layer’s bounds rectangle when drawn.

Default value is `(0.5,1.0)`.

## See Also

### Gradient Style Properties

var colors: [Any]?

An array of `CGColorRef` objects defining the color of each gradient stop. Animatable.

var locations: [NSNumber]?

An optional array of NSNumber objects defining the location of each gradient stop. Animatable.

var startPoint: CGPoint

The start point of the gradient when drawn in the layer’s coordinate space. Animatable.

var type: CAGradientLayerType

Style of gradient drawn by the layer.

