

- ARKit
- SceneReconstructionProvider
-  state 

Instance Property

# state

A value that indicates whether the scene reconstruction provider is currently supplying anchor updates.

visionOS 1.0+

``` source
final var state: DataProviderState { get }
```

## See Also

### Observing scene reconstruction

var anchorUpdates: AnchorUpdateSequence&lt;MeshAnchor>

An asynchronous sequence of updates to scene meshes that the scene reconstruction provider detects.

