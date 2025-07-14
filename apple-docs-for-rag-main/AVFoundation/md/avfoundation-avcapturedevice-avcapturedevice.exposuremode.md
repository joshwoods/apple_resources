

- AVFoundation
- AVCaptureDevice
-  AVCaptureDevice.ExposureMode 

Enumeration

# AVCaptureDevice.ExposureMode

Constants that specify the exposure mode of a capture device.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
enum ExposureMode
```

## Topics

### Exposure Modes

case locked

A mode that locks exposure for the device.

case autoExpose

A mode that automatically adjusts the exposure one time, and then locks exposure for the device.

case continuousAutoExposure

A mode that continuously monitors exposure levels and automatically adjusts exposure when necessary.

case custom

A mode where an app manually sets the exposure duration and ISO values.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing the Exposure Mode

func isExposureModeSupported(AVCaptureDevice.ExposureMode) -> Bool

Returns a Boolean value that indicates whether a device supports the specified exposure mode.

var exposureMode: AVCaptureDevice.ExposureMode

The exposure mode for the device.

