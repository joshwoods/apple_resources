

- RealityKit
- ObjectCaptureSession
- ObjectCaptureSession.CaptureState
-  ObjectCaptureSession.CaptureState.finishing 

Case

# ObjectCaptureSession.CaptureState.finishing

The session is saving outstanding data and finishing up.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
case finishing
```

## Discussion

This state occurs after your app calls finish(). The app should keep the session alive until it reaches `.completed` state to ensure all data has been saved. The session will automatically move to `.completed` once all data is saved.

