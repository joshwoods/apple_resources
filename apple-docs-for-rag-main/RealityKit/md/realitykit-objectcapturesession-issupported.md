

- RealityKit
- ObjectCaptureSession
-  isSupported 

Type Property

# isSupported

A Boolean that indicates whether the current device supports object capture sessions.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
@MainActor
static var isSupported: Bool { get }
```

## Discussion

Before creating an object capture session, check this value to make sure the current device supports the feature. If `false`, attempting to create an `ObjectCaptureSession` will result in a runtime error.

