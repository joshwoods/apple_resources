

- Core Animation
- CAEmitterCell
-  spinRange 

Instance Property

# spinRange

The amount by which the spin of the cell can vary over its lifetime. Animatable.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
var spinRange: CGFloat { get set }
```

## Discussion

The range specifies the mean amount the spin value can vary over the cell’s lifetime.

The default value of this property is `0.0`.

## See Also

### Setting Emitter Cell Motion Attributes

var spin: CGFloat

The rotational velocity, measured in radians per second, to apply to the cell. Animatable.

var emissionLatitude: CGFloat

The latitudinal orientation of the emission angle. Animatable.

var emissionLongitude: CGFloat

The longitudinal orientation of the emission angle. Animatable.

var emissionRange: CGFloat

The angle, in radians, defining a cone around the emission angle. Animatable.

