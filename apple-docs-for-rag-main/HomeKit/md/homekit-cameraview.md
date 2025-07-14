

- HomeKit
-  CameraView 

Structure

# CameraView

A SwiftUI view into which a video stream or an image snapshot is rendered.

HomeKitSwiftUIiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@MainActor @preconcurrency
struct CameraView
```

## Topics

### Creating a camera view

init(source: HMCameraSource)

Creates a new camera view using the given source.

class HMCameraSource

An abstract class for a camera’s data source.

## Relationships

### Conforms To

- Sendable
- View

## See Also

### Managing camera profiles

var cameraProfiles: [HMCameraProfile]?

An array of camera profiles implemented by the accessory.

class HMCameraProfile

A camera profile that interacts with an accessory’s camera.

class HMCameraView

The view into which a video stream or an image snapshot is rendered.

