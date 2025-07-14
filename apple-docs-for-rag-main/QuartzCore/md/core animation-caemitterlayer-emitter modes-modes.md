

- Core Animation
- CAEmitterLayer
-  Emitter Modes 

API Collection

# Emitter Modes

These constants specify the possible emitter modes. They are used by the emitterMode property.

## Topics

### Constants

static let points: CAEmitterLayerEmitterMode

Particles are emitted from points on the particle emitter.

static let outline: CAEmitterLayerEmitterMode

Particles are emitted from the outline of the particle emitter.

static let surface: CAEmitterLayerEmitterMode

Particles are emitted from the surface of the particle emitter.

static let volume: CAEmitterLayerEmitterMode

Particles are emitted from the a position within the particle emitter.

## See Also

### Constants

Emitter Shape

The emission shape is a one, two or three dimensional shape that defines where the emitted particles originate. The shapes are defined by a subset of emitterPosition, emitterZPosition, emitterSize and emitterDepth properties.

Emitter Render Order

These constants specify the order that emitter cells are composited. They are used by the renderMode property.

