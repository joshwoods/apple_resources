

- Core Animation
- CAEmitterLayer
-  birthRate 

Instance Property

# birthRate

Defines a multiplier that is applied to the cell-defined birth rate. Animatable

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
var birthRate: Float { get set }
```

## Discussion

The birth rate of each cell is multiplied by this number to give the actual number of particles created every second. Default value is `1.0`.

## See Also

### Emitter Cell Attribute Multipliers

var scale: Float

Defines a multiplier applied to the cell-defined particle scale.

var seed: UInt32

Specifies the seed used to initialize the random number generator.

var spin: Float

Defines a multiplier applied to the cell-defined particle spin. Animatable.

var velocity: Float

Defines a multiplier applied to the cell-defined particle velocity. Animatable.

var emitterMode: CAEmitterLayerEmitterMode

Specifies the emitter mode.

var lifetime: Float

Defines a multiplier applied to the cell-defined lifetime range when particles are created. Animatable.

var preservesDepth: Bool

Defines whether the layer flattens the particles into its plane.

