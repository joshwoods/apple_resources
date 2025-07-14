

- AVFoundation
- AVCaptureInput
- AVCaptureInput.Port
-  isEnabled 

Instance Property

# isEnabled

A Boolean value that indicates whether the port is in an enabled state.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
var isEnabled: Bool { get set }
```

## Discussion

Ports are in an enabled state by default. If you want to capture only a subset of the media streams provided by a capture input, use this property to selectively disable streams.

## See Also

### Inspecting an Input Port

var mediaType: AVMediaType

The media type of the port.

var formatDescription: CMFormatDescription?

A description of the port format.

var sourceDeviceType: AVCaptureDevice.DeviceType?

The device type of the source camera that provides data to the port.

var sourceDevicePosition: AVCaptureDevice.Position

The position of the source device providing input through this port.

var clock: CMClock?

An object that represents the capture device’s clock.

