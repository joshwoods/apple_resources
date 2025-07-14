

- Core Animation
- CAEmitterLayer
-  seed 

Instance Property

# seed

Specifies the seed used to initialize the random number generator.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
var seed: UInt32 { get set }
```

## Discussion

Each layer has its own random number generator state. Emitter cell properties that are defined as a mean and a range, such as a cell’s `speed`, the value of the properties are uniformly distributed in the interval \[M - R/2, M + R/2\].

## See Also

### Emitter Cell Attribute Multipliers

var scale: Float

Defines a multiplier applied to the cell-defined particle scale.

var spin: Float

Defines a multiplier applied to the cell-defined particle spin. Animatable.

var velocity: Float

Defines a multiplier applied to the cell-defined particle velocity. Animatable.

var birthRate: Float

Defines a multiplier that is applied to the cell-defined birth rate. Animatable

var emitterMode: CAEmitterLayerEmitterMode

Specifies the emitter mode.

var lifetime: Float

Defines a multiplier applied to the cell-defined lifetime range when particles are created. Animatable.

var preservesDepth: Bool

Defines whether the layer flattens the particles into its plane.

