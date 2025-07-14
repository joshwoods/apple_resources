

- Core Animation
- CAEmitterCell
-  emissionRange 

Instance Property

# emissionRange

The angle, in radians, defining a cone around the emission angle. Animatable.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
var emissionRange: CGFloat { get set }
```

## Discussion

Cells are uniformly distributed across this cone.

The default value of this property is `0`.

## See Also

### Setting Emitter Cell Motion Attributes

var spin: CGFloat

The rotational velocity, measured in radians per second, to apply to the cell. Animatable.

var spinRange: CGFloat

The amount by which the spin of the cell can vary over its lifetime. Animatable.

var emissionLatitude: CGFloat

The latitudinal orientation of the emission angle. Animatable.

var emissionLongitude: CGFloat

The longitudinal orientation of the emission angle. Animatable.

