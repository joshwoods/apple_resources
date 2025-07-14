

- RealityKit
- ObjectCaptureSession
-  numberOfShotsTaken 

Instance Property

# numberOfShotsTaken

The number of shots taken in the entire capture session so far, including both automatic capture and manual capture.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
@MainActor
var numberOfShotsTaken: Int { get }
```

## Discussion

This number includes shots from all scan passes, flipped or unflipped. It can be directly compared to the `maximumNumberOfInputImages` to keep track of the memory limits required for reconstruction of this session on-device and whether over-capture mode limits are reached for a given session.

