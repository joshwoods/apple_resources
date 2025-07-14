

- HomeKit
- HMAccessory
-  cameraProfiles 

Instance Property

# cameraProfiles

An array of camera profiles implemented by the accessory.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var cameraProfiles: [HMCameraProfile]? { get }
```

## Discussion

An accessory can contain one or more cameras. Each camera is represented as a an HMCameraProfile instance. If the accessory doesn’t contain a camera, this property is `nil`.

## See Also

### Managing camera profiles

struct CameraView

A SwiftUI view into which a video stream or an image snapshot is rendered.

class HMCameraProfile

A camera profile that interacts with an accessory’s camera.

class HMCameraView

The view into which a video stream or an image snapshot is rendered.

