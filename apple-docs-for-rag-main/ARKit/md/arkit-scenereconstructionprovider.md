

- ARKit
-  SceneReconstructionProvider 

Class

# SceneReconstructionProvider

A source of live data about the shape of a person’s surroundings.

visionOS 1.0+

``` source
final class SceneReconstructionProvider
```

## Topics

### Creating a scene reconstruction provider

init(modes: [SceneReconstructionProvider.Mode])

Creates a provider that reconstructs a person’s surroundings.

let modes: [SceneReconstructionProvider.Mode]

The modes of scene reconstruction a provider supplies.

enum Mode

The additional kinds of information you can request about a person’s surroundings.

static var isSupported: Bool

A Boolean value that indicates whether the current runtime environment supports scene reconstruction providers.

### Observing scene reconstruction

var anchorUpdates: AnchorUpdateSequence&lt;MeshAnchor>

An asynchronous sequence of updates to scene meshes that the scene reconstruction provider detects.

var state: DataProviderState

A value that indicates whether the scene reconstruction provider is currently supplying anchor updates.

### Inspecting a scene reconstruction provider

var description: String

A textual representation of this scene reconstruction provider.

var allAnchors: [MeshAnchor]

An array that contains the mesh anchors the scene reconstruction provider is tracking.

static var requiredAuthorizations: [ARKitSession.AuthorizationType]

The types of authorizations necessary for running scene reconstruction.

## Relationships

### Conforms To

- CustomStringConvertible
- DataProvider
- Sendable

## See Also

### Scene reconstruction

Incorporating real-world surroundings in an immersive experience

Create an immersive experience by making your app’s content respond to the local shape of the world.

struct MeshAnchor

A volume of space that contains a mesh of a person’s surroundings.

