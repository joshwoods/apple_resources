

- RealityKit
- ObjectCaptureSession
-  canRequestImageCapture 

Instance Property

# canRequestImageCapture

Will be `true` only when a call to requestImageCapture() is expected to be successful. It will be `false` when not in the `.capturing` state or if the session is too busy to currently process a new request. There is a period of time after requesting an image capture where this property will be `false` and a new call to requestImageCapture() will not produce a new image.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
@MainActor
var canRequestImageCapture: Bool { get }
```

