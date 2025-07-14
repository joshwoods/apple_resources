

- RealityKit
- ObjectCaptureSession
- ObjectCaptureSession.Tracking
-  ObjectCaptureSession.Tracking.limited(reason:) 

Case

# ObjectCaptureSession.Tracking.limited(reason:)

Tracking is available but its quality is degraded. The ARKit coaching overlay will appear when cameraTracking enters this state.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
case limited(reason: ObjectCaptureSession.Tracking.Reason)
```

## Parameters 

`reason`  

Why tracking is currently degraded.

