

- Core Animation
- CAEmitterLayer
-  emitterZPosition 

Instance Property

# emitterZPosition

Specifies the center of the particle emitter shape along the z-axis. Animatable.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
var emitterZPosition: CGFloat { get set }
```

## Discussion

See Emitter Shape for details of how the emitterZPosition relates to the possible emitter shapes.

Default is `0.0`.

## See Also

### Emitter Geometry

var renderMode: CAEmitterLayerRenderMode

Defines how particle cells are rendered into the layer.

var emitterPosition: CGPoint

The position of the center of the particle emitter. Animatable.

var emitterShape: CAEmitterLayerEmitterShape

Specifies the emitter shape.

var emitterDepth: CGFloat

Determines the depth of the emitter shape.

var emitterSize: CGSize

Determines the size of the particle emitter shape. Animatable.

