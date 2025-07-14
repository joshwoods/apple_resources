

- Core Animation
-  CAEmitterLayer 

Class

# CAEmitterLayer

A layer that emits, animates, and renders a particle system.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
class CAEmitterLayer
```

## Overview

The particles, defined by instances of CAEmitterCell, are drawn above the layer’s background color and border.

The following code shows how to set up a simple point (the default emitterShape is point) particle emitter. It uses an image named `RadialGradient.png` as the cell contents and, by setting the emitter cell’s emissionRange to `2 x` doc://com.apple.documentation/documentation/corefoundation/cgfloat/1845230-pi, the particles are emitted in all directions.

```
let emitterLayer = CAEmitterLayer()

emitterLayer.emitterPosition = CGPoint(x: 320, y: 320)

let cell = CAEmitterCell()
cell.birthRate = 100
cell.lifetime = 10
cell.velocity = 100
cell.scale = 0.1

cell.emissionRange = CGFloat.pi * 2.0
cell.contents = UIImage(named: "RadialGradient.png")!.cgImage

emitterLayer.emitterCells = [cell]

view.layer.addSublayer(emitterLayer)
```

## Topics

### Specifying Particle Emitter Cells

var emitterCells: [CAEmitterCell]?

The array emitter cells attached to the layer.

### Emitter Geometry

var renderMode: CAEmitterLayerRenderMode

Defines how particle cells are rendered into the layer.

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

var preservesDepth: Bool

Defines whether the layer flattens the particles into its plane.

### Constants

Emitter Shape

The emission shape is a one, two or three dimensional shape that defines where the emitted particles originate. The shapes are defined by a subset of emitterPosition, emitterZPosition, emitterSize and emitterDepth properties.

Emitter Modes

These constants specify the possible emitter modes. They are used by the emitterMode property.

Emitter Render Order

These constants specify the order that emitter cells are composited. They are used by the renderMode property.

## Relationships

### Inherits From

- CALayer

### Conforms To

- CAMediaTiming
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Particle Systems

class CAEmitterCell

The definition of a particle emitted by a particle layer.

