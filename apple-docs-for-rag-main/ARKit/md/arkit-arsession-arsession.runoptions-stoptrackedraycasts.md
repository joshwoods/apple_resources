

- ARKit
- ARSession
- ARSession.RunOptions
-  stopTrackedRaycasts 

Type Property

# stopTrackedRaycasts

An option to stop all active tracked raycasts.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
static var stopTrackedRaycasts: ARSession.RunOptions { get }
```

## Discussion

By default, when you call the run(_:options:) method on a session that is running or has run before, the session keeps tracking any ARTrackedRaycast objects that you previously added by calling trackedRaycast(_:updateHandler:).

Use stopTrackedRaycasts if you want to stop all active tracked raycasts. Alternatively, you can stop individual raycasts by calling stopTracking() on individual raycasts.

## See Also

### Run Options

static var resetTracking: ARSession.RunOptions

An option to reset the device’s position from the session’s previous run.

static var removeExistingAnchors: ARSession.RunOptions

An option to remove any anchor objects associated with the session’s previous run.

static var resetSceneReconstruction: ARSession.RunOptions

An option to reset the scene mesh.

