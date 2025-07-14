

- ARKit
- ARSession
- ARSession.RunOptions
-  removeExistingAnchors 

Type Property

# removeExistingAnchors

An option to remove any anchor objects associated with the session’s previous run.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
static var removeExistingAnchors: ARSession.RunOptions { get }
```

## Discussion

By default, when you call the run(_:options:) method on a session that has run before or is already running, the session keeps any ARAnchor objects that you previously added. That is, objects in the AR scene keep their apparent real-world positions relative to the device (unless you enable the resetTracking option).

Enable the removeExistingAnchors option if changing session configurations should invalidate the apparent real-world positions of objects in the AR scene. For example, if you’ve added virtual content to the AR scene whose positions are correlated to real-world objects, remove those anchors so you can reevaluate appropriate real-world positions. On the other hand, if the virtual content in your scene needs to track real-world positions only when that content first appears and can move freely thereafter, you can disable this option to keep the anchors.

## See Also

### Run Options

static var resetTracking: ARSession.RunOptions

An option to reset the device’s position from the session’s previous run.

static var stopTrackedRaycasts: ARSession.RunOptions

An option to stop all active tracked raycasts.

static var resetSceneReconstruction: ARSession.RunOptions

An option to reset the scene mesh.

