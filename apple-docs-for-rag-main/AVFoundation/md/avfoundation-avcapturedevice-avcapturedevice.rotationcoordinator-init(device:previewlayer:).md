

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.RotationCoordinator
-  init(device:previewLayer:) 

Initializer

# init(device:previewLayer:)

Creates a coordinator that provides separate compensation angles for content your app takes with a capture device, and for your app’s camera preview.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
init(
    device: AVCaptureDevice,
    previewLayer: CALayer?
)
```

## Parameters 

`device`  

A capture device the new coordinator monitors to track its physical rotation to calculate its videoRotationAngleForHorizonLevelCapture property.

`previewLayer`  

A layer that displays a camera preview the new coordinator monitors to calculate its videoRotationAngleForHorizonLevelPreview property.

