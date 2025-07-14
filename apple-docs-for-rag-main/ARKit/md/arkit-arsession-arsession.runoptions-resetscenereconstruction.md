

- ARKit
- ARSession
- ARSession.RunOptions
-  resetSceneReconstruction 

Type Property

# resetSceneReconstruction

An option to reset the scene mesh.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
static var resetSceneReconstruction: ARSession.RunOptions { get }
```

## Discussion

When you reset scene reconstruction, ARKit removes any existing mesh anchors (ARMeshAnchor) from the session.

## See Also

### Run Options

static var resetTracking: ARSession.RunOptions

An option to reset the device’s position from the session’s previous run.

static var removeExistingAnchors: ARSession.RunOptions

An option to remove any anchor objects associated with the session’s previous run.

static var stopTrackedRaycasts: ARSession.RunOptions

An option to stop all active tracked raycasts.

