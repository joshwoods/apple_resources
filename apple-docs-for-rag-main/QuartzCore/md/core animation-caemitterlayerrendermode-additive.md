

- Core Animation
- CAEmitterLayerRenderMode
-  additive 

Type Property

# additive

The particles are rendered using source-additive compositing.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
static let additive: CAEmitterLayerRenderMode
```

## See Also

### Constants

static let unordered: CAEmitterLayerRenderMode

Particles are rendered unordered. This mode uses source-over compositing.

static let oldestFirst: CAEmitterLayerRenderMode

Particles are rendered oldest first. This mode uses source-over compositing.

static let oldestLast: CAEmitterLayerRenderMode

Particles are rendered oldest last. This mode uses source-over compositing.

static let backToFront: CAEmitterLayerRenderMode

Particles are rendered from back to front, sorted by z-position. This mode uses source-over compositing.

