

- ARKit
- SceneReconstructionProvider
-  allAnchors 

Instance Property

# allAnchors

An array that contains the mesh anchors the scene reconstruction provider is tracking.

visionOS 2.0+

``` source
final var allAnchors: [MeshAnchor] { get }
```

## See Also

### Inspecting a scene reconstruction provider

var description: String

A textual representation of this scene reconstruction provider.

static var requiredAuthorizations: [ARKitSession.AuthorizationType]

The types of authorizations necessary for running scene reconstruction.

