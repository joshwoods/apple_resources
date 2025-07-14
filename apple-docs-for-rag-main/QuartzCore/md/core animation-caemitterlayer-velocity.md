

- Core Animation
- CAEmitterLayer
-  velocity 

Instance Property

# velocity

Defines a multiplier applied to the cell-defined particle velocity. Animatable.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
var velocity: Float { get set }
```

## Discussion

Default value is `1.0`.

## See Also

### Emitter Cell Attribute Multipliers

var scale: Float

Defines a multiplier applied to the cell-defined particle scale.

var seed: UInt32

Specifies the seed used to initialize the random number generator.

var spin: Float

Defines a multiplier applied to the cell-defined particle spin. Animatable.

var birthRate: Float

Defines a multiplier that is applied to the cell-defined birth rate. Animatable

var emitterMode: CAEmitterLayerEmitterMode

Specifies the emitter mode.

var lifetime: Float

Defines a multiplier applied to the cell-defined lifetime range when particles are created. Animatable.

var preservesDepth: Bool

Defines whether the layer flattens the particles into its plane.

