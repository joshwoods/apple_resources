

- RealityKit
- ObjectCaptureSession
- ObjectCaptureSession.CaptureState
-  ObjectCaptureSession.CaptureState.capturing 

Case

# ObjectCaptureSession.CaptureState.capturing

Auto-capture is in progress.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
case capturing
```

## Discussion

In this state the user is expected to orbit the device slowly and smoothly around the object in order to fully complete the capture dial.

In this state an app may also manually request captures with a call to requestImageCapture().

