

- ARKit
- SceneReconstructionProvider
-  anchorUpdates 

Instance Property

# anchorUpdates

An asynchronous sequence of updates to scene meshes that the scene reconstruction provider detects.

visionOS 1.0+

``` source
final var anchorUpdates: AnchorUpdateSequence { get }
```

## See Also

### Observing scene reconstruction

var state: DataProviderState

A value that indicates whether the scene reconstruction provider is currently supplying anchor updates.

