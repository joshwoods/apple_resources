

- RealityKit
- ObjectCaptureSession
- ObjectCaptureSession.CaptureState
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Two states are defined equal if they have the same case. Specifically, a `.failed(Error)` state will match any other failed state regardless of the actual error payload.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
static func == (lhs: ObjectCaptureSession.CaptureState, rhs: ObjectCaptureSession.CaptureState) -> Bool
```

