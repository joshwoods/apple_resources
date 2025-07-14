

- Core Animation
- CAEmitterCell
-  emissionLongitude 

Instance Property

# emissionLongitude

The longitudinal orientation of the emission angle. Animatable.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
var emissionLongitude: CGFloat { get set }
```

## Discussion

The emission longitude is the orientation of the emission angle in the xy-plane. it is also often referred to as the azimuth.

The default value of this property is `0.0`.

## See Also

### Setting Emitter Cell Motion Attributes

var spin: CGFloat

The rotational velocity, measured in radians per second, to apply to the cell. Animatable.

var spinRange: CGFloat

The amount by which the spin of the cell can vary over its lifetime. Animatable.

var emissionLatitude: CGFloat

The latitudinal orientation of the emission angle. Animatable.

var emissionRange: CGFloat

The angle, in radians, defining a cone around the emission angle. Animatable.

