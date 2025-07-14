

- Core Animation
- CAEmitterLayer
-  preservesDepth 

Instance Property

# preservesDepth

Defines whether the layer flattens the particles into its plane.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
var preservesDepth: Bool { get set }
```

## Discussion

If true, the layer renders its particles as if they directly inhabit the three-dimensional coordinate space of the layer’s superlayer. When enabled, the effect of the layer’s `filters`, `backgroundFilters`, and shadow related properties is undefined.

Default is false.

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

var emitterMode: CAEmitterLayerEmitterMode

Specifies the emitter mode.

var lifetime: Float

Defines a multiplier applied to the cell-defined lifetime range when particles are created. Animatable.

