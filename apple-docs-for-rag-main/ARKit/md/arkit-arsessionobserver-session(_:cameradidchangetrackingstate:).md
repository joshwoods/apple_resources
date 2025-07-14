

- ARKit
- ARSessionObserver
-  session(\_:cameraDidChangeTrackingState:) 

Instance Method

# session(\_:cameraDidChangeTrackingState:)

Informs the delegate of changes to the quality of ARKit’s device position tracking.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
optional func session(
    _ session: ARSession,
    cameraDidChangeTrackingState camera: ARCamera
)
```

## Parameters 

`session`  

The session providing information.

`camera`  

The camera whose tracking parameters have changed. (Equivalent to currentFrame.camera.)

## Discussion

ARKit tracks the position and orientation of the device relative to a virtual scene through a combination of motion sensing and image processing. As such, factors that affect signal quality from the device’s motion sensing hardware or that interfere with scene detection in the camera image can result in poor estimates of the device position relative to the virtual scene.

## See Also

### Responding to Tracking Quality Changes

func session(ARSession, didChange: ARGeoTrackingStatus)

Listen and react to geo-tracking state changes.

