

- Core Animation
- CAEmitterLayer
-  Emitter Shape 

API Collection

# Emitter Shape

The emission shape is a one, two or three dimensional shape that defines where the emitted particles originate. The shapes are defined by a subset of emitterPosition, emitterZPosition, emitterSize and emitterDepth properties.

## Topics

### Constants

static let point: CAEmitterLayerEmitterShape

Particles are emitted from a single point at (`emitterPosition.x`, `emitterPosition.y`, `emitterZPosition`)

static let line: CAEmitterLayerEmitterShape

Particles are emitted along a line from (`emitterPosition.x - emitterSize.width/2`, `emitterPosition.y`, `emitterZPosition`) to (`emitterPosition.x + emitterSize.width/2`, `emitterPosition.y`, `emitterZPosition`).

static let rectangle: CAEmitterLayerEmitterShape

Particles are emitted from a rectangle with opposite corners \[emitterPosition.x - emitterSize.width/2, emitterPosition.y - emitterSize.height/2, emitterZPosition\], \[emitterPosition.x + emitterSize.width/2, emitterPosition.y + emitterSize.height/2, emitterZPosition\].

static let cuboid: CAEmitterLayerEmitterShape

Particles are emitted from a cuboid (3D rectangle) with opposite corners: \[emitterPosition.x - emitterSize.width/2, emitterPosition.y - emitterSize.height/2, emitterZPosition - emitterDepth/2\], \[emitterPosition.x + emitterSize.width/2, emitterPosition.y + emitterSize.height/2, emitterZPosition+emitterDepth/2\].

static let circle: CAEmitterLayerEmitterShape

Particles are emitted from a circle centered at (`emitterPosition.x`, `emitterPosition.y`, `emitterZPosition`) of radius `emitterSize.width`.

static let sphere: CAEmitterLayerEmitterShape

Particles are emitted from a sphere centered at (`emitterPosition.x`, `emitterPosition.y`, `emitterZPosition`) of radius `emitterSize.width`.

## See Also

### Constants

Emitter Modes

These constants specify the possible emitter modes. They are used by the emitterMode property.

Emitter Render Order

These constants specify the order that emitter cells are composited. They are used by the renderMode property.

