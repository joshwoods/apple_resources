

- Core Animation
- CAEmitterLayer
-  emitterShape 

Instance Property

# emitterShape

Specifies the emitter shape.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
var emitterShape: CAEmitterLayerEmitterShape { get set }
```

## Discussion

The possible values for emitterMode are shown in Emitter Shape. The default value is point.

## See Also

### Emitter Geometry

var renderMode: CAEmitterLayerRenderMode

Defines how particle cells are rendered into the layer.

var emitterPosition: CGPoint

The position of the center of the particle emitter. Animatable.

var emitterZPosition: CGFloat

Specifies the center of the particle emitter shape along the z-axis. Animatable.

var emitterDepth: CGFloat

Determines the depth of the emitter shape.

var emitterSize: CGSize

Determines the size of the particle emitter shape. Animatable.

