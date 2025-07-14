

- AVFoundation
- AVCaptureInput
- AVCaptureInput.Port
-  clock 

Instance Property

# clock

An object that represents the capture device’s clock.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+macOS 10.9+tvOS 17.0+

``` source
var clock: CMClock? { get }
```

## Discussion

The value of this property is readonly and may not reflect the actual clock in the capture device.

## See Also

### Inspecting an Input Port

var isEnabled: Bool

A Boolean value that indicates whether the port is in an enabled state.

var mediaType: AVMediaType

The media type of the port.

var formatDescription: CMFormatDescription?

A description of the port format.

var sourceDeviceType: AVCaptureDevice.DeviceType?

The device type of the source camera that provides data to the port.

var sourceDevicePosition: AVCaptureDevice.Position

The position of the source device providing input through this port.

