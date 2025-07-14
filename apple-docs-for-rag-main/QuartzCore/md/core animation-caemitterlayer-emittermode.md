

- Core Animation
- CAEmitterLayer
-  emitterMode 

Instance Property

# emitterMode

Specifies the emitter mode.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
var emitterMode: CAEmitterLayerEmitterMode { get set }
```

## Discussion

The possible values for emitterMode are shown in Emitter Modes. The default value is volume.

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

var birthRate: Float

Defines a multiplier that is applied to the cell-defined birth rate. Animatable

var lifetime: Float

Defines a multiplier applied to the cell-defined lifetime range when particles are created. Animatable.

var preservesDepth: Bool

Defines whether the layer flattens the particles into its plane.

