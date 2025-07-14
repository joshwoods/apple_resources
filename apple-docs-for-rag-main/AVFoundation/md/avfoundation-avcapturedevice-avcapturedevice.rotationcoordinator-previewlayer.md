

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.RotationCoordinator
-  previewLayer 

Instance Property

# previewLayer

The layer that displays a camera preview the coordinator calculates a video rotation angle for.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
weak var previewLayer: CALayer? { get }
```

## Discussion

The coordinator updates its videoRotationAngleForHorizonLevelPreview property by monitoring the layer and the physical rotation of device.

## See Also

### Inspecting a coordinator’s configuration

var device: AVCaptureDevice?

The capture device the coordinator monitors to track its physical rotation.

