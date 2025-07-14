

- RealityKit
- ObjectCaptureSession
- ObjectCaptureSession.Configuration
-  isOverCaptureEnabled 

Instance Property

# isOverCaptureEnabled

Enables the session to continue capturing even after the number of captured images exceeds `maximumNumberOfInputImages`. This setting is meant for use when the images are intended to be transferred to macOS for model reconstruction.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
var isOverCaptureEnabled: Bool
```

## Discussion

Note: The number of images used for on-device reconstruction will be limited to `maximumNumberOfInputImages` with any extra images skipped.

