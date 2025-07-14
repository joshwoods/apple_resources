

- Core Animation
- CAEmitterLayer
-  emitterDepth 

Instance Property

# emitterDepth

Determines the depth of the emitter shape.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
var emitterDepth: CGFloat { get set }
```

## Discussion

How the emitter depth is applied depends on the emitter shape. See Emitter Shape for details. Depending on the value of emitterShape, this value may be ignored.

Default is `0.0`.

## See Also

### Emitter Geometry

var renderMode: CAEmitterLayerRenderMode

Defines how particle cells are rendered into the layer.

var emitterPosition: CGPoint

The position of the center of the particle emitter. Animatable.

var emitterShape: CAEmitterLayerEmitterShape

Specifies the emitter shape.

var emitterZPosition: CGFloat

Specifies the center of the particle emitter shape along the z-axis. Animatable.

var emitterSize: CGSize

Determines the size of the particle emitter shape. Animatable.

