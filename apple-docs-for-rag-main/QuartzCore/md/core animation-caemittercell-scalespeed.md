

- Core Animation
- CAEmitterCell
-  scaleSpeed 

Instance Property

# scaleSpeed

The speed at which the scale changes over the lifetime of the cell. Animatable.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
var scaleSpeed: CGFloat { get set }
```

## Discussion

The speed change is defined as the rate of change per second.

The default value of this property is `0.0`.

## See Also

### Setting Emitter Cell Temporal Attributes

var lifetime: Float

The lifetime of the cell, in seconds. Animatable.

var lifetimeRange: Float

The mean value by which the lifetime of the cell can vary. Animatable.

var birthRate: Float

The number of emitted objects created every second. Animatable.

var velocity: CGFloat

The initial velocity of the cell. Animatable.

var velocityRange: CGFloat

The amount by which the velocity of the cell can vary. Animatable.

var xAcceleration: CGFloat

The x component of an acceleration vector applied to cell.

var yAcceleration: CGFloat

The y component of an acceleration vector applied to cell.

var zAcceleration: CGFloat

The z component of an acceleration vector applied to cell.

