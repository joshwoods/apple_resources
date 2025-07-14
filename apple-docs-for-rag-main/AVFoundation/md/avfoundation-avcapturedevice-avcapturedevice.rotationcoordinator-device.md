

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.RotationCoordinator
-  device 

Instance Property

# device

The capture device the coordinator monitors to track its physical rotation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
weak var device: AVCaptureDevice? { get }
```

## Discussion

The coordinator updates its videoRotationAngleForHorizonLevelCapture property by monitoring the device’s physical rotation.

## See Also

### Inspecting a coordinator’s configuration

var previewLayer: CALayer?

The layer that displays a camera preview the coordinator calculates a video rotation angle for.

