

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.LensStabilizationStatus
-  AVCaptureDevice.LensStabilizationStatus.unsupported 

Case

# AVCaptureDevice.LensStabilizationStatus.unsupported

Lens stabilization isn’t available on the device or device configuration that captured this photo.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
case unsupported
```

## See Also

### Lens Stabilization Values

case off

Lens stabilization isn’t specified for this photo capture.

case active

Lens stabilization was active for the full duration of the photo capture.

case outOfRange

Lens stabilization was enabled for the photo capture, but device motion or capture duration exceeded the stabilization module’s correction limits.

case unavailable

Lens stabilization was temporarily unavailable during the photo capture.

