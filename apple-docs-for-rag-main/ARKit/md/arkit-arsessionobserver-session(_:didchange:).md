

- ARKit
- ARSessionObserver
-  session(\_:didChange:) 

Instance Method

# session(\_:didChange:)

Listen and react to geo-tracking state changes.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
optional func session(
    _ session: ARSession,
    didChange geoTrackingStatus: ARGeoTrackingStatus
)
```

## Parameters 

`session`  

The geo-tracking session.

`geoTrackingStatus`  

The new status.

## Discussion

To create and maintain an effective geo-tracking session, an app must react promptly when ARKit changes the geo-tracking status. For more information, see ARGeoTrackingStatus.

ARKit invokes this callback only for ARGeoTrackingConfiguration sessions.

## See Also

### Responding to Tracking Quality Changes

func session(ARSession, cameraDidChangeTrackingState: ARCamera)

Informs the delegate of changes to the quality of ARKit’s device position tracking.

