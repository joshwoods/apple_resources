

- AVFoundation
- AVCaptureInput
- AVCaptureInput.Port
-  mediaType 

Instance Property

# mediaType

The media type of the port.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
var mediaType: AVMediaType { get }
```

## See Also

### Inspecting an Input Port

var isEnabled: Bool

A Boolean value that indicates whether the port is in an enabled state.

var formatDescription: CMFormatDescription?

A description of the port format.

var sourceDeviceType: AVCaptureDevice.DeviceType?

The device type of the source camera that provides data to the port.

var sourceDevicePosition: AVCaptureDevice.Position

The position of the source device providing input through this port.

var clock: CMClock?

An object that represents the capture device’s clock.

