

- RealityKit
- ARView
-  environment 

Instance Property

# environment

The view’s background, lighting, and acoustic properties.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+

``` source
@MainActor @preconcurrency
var environment: ARView.Environment { get set }
```

## See Also

### Providing environmental context

var physicsOrigin: Entity?

The entity that defines the origin of the scene’s physics simulation.

var audioListener: Entity?

The entity that defines the listener position and orientation for spatial audio.

