

- Core Animation
- CAEmitterLayer
-  renderMode 

Instance Property

# renderMode

Defines how particle cells are rendered into the layer.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
var renderMode: CAEmitterLayerRenderMode { get set }
```

## Discussion

The possible values for render modes are shown in Emitter Modes. The default value is unordered.

## See Also

### Emitter Geometry

var emitterPosition: CGPoint

The position of the center of the particle emitter. Animatable.

var emitterShape: CAEmitterLayerEmitterShape

Specifies the emitter shape.

var emitterZPosition: CGFloat

Specifies the center of the particle emitter shape along the z-axis. Animatable.

var emitterDepth: CGFloat

Determines the depth of the emitter shape.

var emitterSize: CGSize

Determines the size of the particle emitter shape. Animatable.

