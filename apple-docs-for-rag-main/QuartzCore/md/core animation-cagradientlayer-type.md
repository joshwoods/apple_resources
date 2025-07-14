

- Core Animation
- CAGradientLayer
-  type 

Instance Property

# type

Style of gradient drawn by the layer.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
var type: CAGradientLayerType { get set }
```

## Discussion

Defaults to axial.

## See Also

### Gradient Style Properties

var colors: [Any]?

An array of `CGColorRef` objects defining the color of each gradient stop. Animatable.

var locations: [NSNumber]?

An optional array of NSNumber objects defining the location of each gradient stop. Animatable.

var endPoint: CGPoint

The end point of the gradient when drawn in the layer’s coordinate space. Animatable.

var startPoint: CGPoint

The start point of the gradient when drawn in the layer’s coordinate space. Animatable.

