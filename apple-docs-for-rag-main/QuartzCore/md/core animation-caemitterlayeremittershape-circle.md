

- Core Animation
- CAEmitterLayerEmitterShape
-  circle 

Type Property

# circle

Particles are emitted from a circle centered at (`emitterPosition.x`, `emitterPosition.y`, `emitterZPosition`) of radius `emitterSize.width`.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
static let circle: CAEmitterLayerEmitterShape
```

## See Also

### Constants

static let point: CAEmitterLayerEmitterShape

Particles are emitted from a single point at (`emitterPosition.x`, `emitterPosition.y`, `emitterZPosition`)

static let line: CAEmitterLayerEmitterShape

Particles are emitted along a line from (`emitterPosition.x - emitterSize.width/2`, `emitterPosition.y`, `emitterZPosition`) to (`emitterPosition.x + emitterSize.width/2`, `emitterPosition.y`, `emitterZPosition`).

static let rectangle: CAEmitterLayerEmitterShape

Particles are emitted from a rectangle with opposite corners \[emitterPosition.x - emitterSize.width/2, emitterPosition.y - emitterSize.height/2, emitterZPosition\], \[emitterPosition.x + emitterSize.width/2, emitterPosition.y + emitterSize.height/2, emitterZPosition\].

static let cuboid: CAEmitterLayerEmitterShape

Particles are emitted from a cuboid (3D rectangle) with opposite corners: \[emitterPosition.x - emitterSize.width/2, emitterPosition.y - emitterSize.height/2, emitterZPosition - emitterDepth/2\], \[emitterPosition.x + emitterSize.width/2, emitterPosition.y + emitterSize.height/2, emitterZPosition+emitterDepth/2\].

static let sphere: CAEmitterLayerEmitterShape

Particles are emitted from a sphere centered at (`emitterPosition.x`, `emitterPosition.y`, `emitterZPosition`) of radius `emitterSize.width`.

