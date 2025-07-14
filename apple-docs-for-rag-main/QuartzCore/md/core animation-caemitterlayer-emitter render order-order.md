

- Core Animation
- CAEmitterLayer
-  Emitter Render Order 

API Collection

# Emitter Render Order

These constants specify the order that emitter cells are composited. They are used by the renderMode property.

## Topics

### Constants

static let unordered: CAEmitterLayerRenderMode

Particles are rendered unordered. This mode uses source-over compositing.

static let oldestFirst: CAEmitterLayerRenderMode

Particles are rendered oldest first. This mode uses source-over compositing.

static let oldestLast: CAEmitterLayerRenderMode

Particles are rendered oldest last. This mode uses source-over compositing.

static let backToFront: CAEmitterLayerRenderMode

Particles are rendered from back to front, sorted by z-position. This mode uses source-over compositing.

static let additive: CAEmitterLayerRenderMode

The particles are rendered using source-additive compositing.

## See Also

### Constants

Emitter Shape

The emission shape is a one, two or three dimensional shape that defines where the emitted particles originate. The shapes are defined by a subset of emitterPosition, emitterZPosition, emitterSize and emitterDepth properties.

Emitter Modes

These constants specify the possible emitter modes. They are used by the emitterMode property.

