

- ARKit
- ARSession
- ARSession.RunOptions
-  resetTracking 

Type Property

# resetTracking

An option to reset the device’s position from the session’s previous run.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
static var resetTracking: ARSession.RunOptions { get }
```

## Mentioned in 

Managing Session Life Cycle and Tracking Quality

## Discussion

By default, when you call the run(_:options:) method on a session that has run before or is already running, the session resumes device position tracking from its last known state. (For example, an ARAnchor object keeps its apparent position relative to the camera.) When you call the run(_:options:) method with a configuration of the same type as the session’s current configuration, you can add this option to force device position tracking to return to its initial state.

When you call the run(_:options:) method with a configuration of a different type than the session’s current configuration, the session always resets tracking (that is, this option is implicitly enabled).

In either case, when you reset tracking, ARKit also removes any existing anchors from the session.

## See Also

### Run Options

static var removeExistingAnchors: ARSession.RunOptions

An option to remove any anchor objects associated with the session’s previous run.

static var stopTrackedRaycasts: ARSession.RunOptions

An option to stop all active tracked raycasts.

static var resetSceneReconstruction: ARSession.RunOptions

An option to reset the scene mesh.

