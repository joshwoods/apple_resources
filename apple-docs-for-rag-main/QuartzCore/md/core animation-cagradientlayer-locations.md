

- Core Animation
- CAGradientLayer
-  locations 

Instance Property

# locations

An optional array of NSNumber objects defining the location of each gradient stop. Animatable.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
var locations: [NSNumber]? { get set }
```

## Discussion

The gradient stops are specified as values between `0` and `1`. The values must be monotonically increasing. If `nil`, the stops are spread uniformly across the range. Defaults to `nil`.

When rendered, the colors are mapped to the output color space before being interpolated.

## See Also

### Gradient Style Properties

var colors: [Any]?

An array of `CGColorRef` objects defining the color of each gradient stop. Animatable.

var endPoint: CGPoint

The end point of the gradient when drawn in the layer’s coordinate space. Animatable.

var startPoint: CGPoint

The start point of the gradient when drawn in the layer’s coordinate space. Animatable.

var type: CAGradientLayerType

Style of gradient drawn by the layer.

