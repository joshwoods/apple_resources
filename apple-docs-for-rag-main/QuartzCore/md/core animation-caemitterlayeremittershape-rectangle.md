

- Core Animation
- CAEmitterLayerEmitterShape
-  rectangle 

Type Property

# rectangle

Particles are emitted from a rectangle with opposite corners \[emitterPosition.x - emitterSize.width/2, emitterPosition.y - emitterSize.height/2, emitterZPosition\], \[emitterPosition.x + emitterSize.width/2, emitterPosition.y + emitterSize.height/2, emitterZPosition\].

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
static let rectangle: CAEmitterLayerEmitterShape
```

## See Also

### Constants

static let point: CAEmitterLayerEmitterShape

Particles are emitted from a single point at (`emitterPosition.x`, `emitterPosition.y`, `emitterZPosition`)

static let line: CAEmitterLayerEmitterShape

Particles are emitted along a line from (`emitterPosition.x - emitterSize.width/2`, `emitterPosition.y`, `emitterZPosition`) to (`emitterPosition.x + emitterSize.width/2`, `emitterPosition.y`, `emitterZPosition`).

static let cuboid: CAEmitterLayerEmitterShape

Particles are emitted from a cuboid (3D rectangle) with opposite corners: \[emitterPosition.x - emitterSize.width/2, emitterPosition.y - emitterSize.height/2, emitterZPosition - emitterDepth/2\], \[emitterPosition.x + emitterSize.width/2, emitterPosition.y + emitterSize.height/2, emitterZPosition+emitterDepth/2\].

static let circle: CAEmitterLayerEmitterShape

Particles are emitted from a circle centered at (`emitterPosition.x`, `emitterPosition.y`, `emitterZPosition`) of radius `emitterSize.width`.

static let sphere: CAEmitterLayerEmitterShape

Particles are emitted from a sphere centered at (`emitterPosition.x`, `emitterPosition.y`, `emitterZPosition`) of radius `emitterSize.width`.

