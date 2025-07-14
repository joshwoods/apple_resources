

- Core Animation
- CAEmitterLayer
-  emitterPosition 

Instance Property

# emitterPosition

The position of the center of the particle emitter. Animatable.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
var emitterPosition: CGPoint { get set }
```

## Discussion

See Emitter Shape for details of how the `emitterPosition` relates to the possible emitter shapes.

Default is `(0.0,0.0)`.

## See Also

### Emitter Geometry

var renderMode: CAEmitterLayerRenderMode

Defines how particle cells are rendered into the layer.

var emitterShape: CAEmitterLayerEmitterShape

Specifies the emitter shape.

var emitterZPosition: CGFloat

Specifies the center of the particle emitter shape along the z-axis. Animatable.

var emitterDepth: CGFloat

Determines the depth of the emitter shape.

var emitterSize: CGSize

Determines the size of the particle emitter shape. Animatable.

