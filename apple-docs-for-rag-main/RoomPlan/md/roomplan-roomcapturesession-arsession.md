

- RoomPlan
- RoomCaptureSession
-  arSession 

Instance Property

# arSession

An object that manages an ARKit session.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
var arSession: ARSession
```

## Discussion

You may use this object to display your own AR experience.

RoomCaptureSession sets this property at initialization and throws an error if your app attempts to set a value.

