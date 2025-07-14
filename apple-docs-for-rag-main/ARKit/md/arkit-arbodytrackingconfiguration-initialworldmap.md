

- ARKit
- ARBodyTrackingConfiguration
-  initialWorldMap 

Instance Property

# initialWorldMap

The state from a previous AR session to attempt to resume with this session configuration.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var initialWorldMap: ARWorldMap? { get set }
```

## Discussion

An ARWorldMap encapsulates the state of a running ARSession. This state includes ARKit’s awareness of the physical space the user moves the device in (which ARKit uses to determine the device’s position and orientation), as well as any ARAnchor objects added to the session (which can represent detected real-world features or virtual content placed by your app). After you use getCurrentWorldMap(completionHandler:) to save a session’s world map, you can assign it to a configuration’s initialWorldMap property and use run(_:options:) to start another session with the same spatial awareness and anchors.

By saving world maps and using them to start new sessions, your app can add new AR capabilities:

- **Multiuser AR experiences.** Create a shared frame of reference by sending archived ARWorldMap objects to a nearby user’s device. With two devices tracking the same world map, you can build a networked experience where both users can see and interact with the same virtual content.

- **Persistent AR experiences.** Save a world map when your app becomes inactive, then restore it the next time your app launches in the same physical environment. You can use anchors from the resumed world map to place the same virtual content at the same positions from the saved session.

When you run a session with an initial world map, the session starts in the ARCamera.TrackingState.limited(_:) (ARCamera.TrackingState.Reason.relocalizing) tracking state while ARKit attempts to reconcile the recorded world map with the current environment. If successful, the tracking state becomes ARCamera.TrackingState.normal after a short time, indicating that the current world coordinate system and anchors match those from the recorded world map.

If ARKit cannot reconcile the recorded world map with the current environment (for example, if the device is in an entirely different place from where the world map was recorded), the session remains in the ARCamera.TrackingState.Reason.relocalizing state indefinitely.

## See Also

### Creating a Configuration

init()

Creates a new body tracking configuration.

