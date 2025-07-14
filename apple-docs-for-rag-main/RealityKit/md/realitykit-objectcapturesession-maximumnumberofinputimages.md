

- RealityKit
- ObjectCaptureSession
-  maximumNumberOfInputImages 

Instance Property

# maximumNumberOfInputImages

The maximum number of images that can be used for on-device reconstruction.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
@MainActor
var maximumNumberOfInputImages: Int { get }
```

## Discussion

Note: the session will stop capturing images when this limit is reached unless isOverCaptureEnabled is true.

