

- AVFoundation
- AVCaptureInput
- AVCaptureInput.Port
-  sourceDeviceType 

Instance Property

# sourceDeviceType

The device type of the source camera that provides data to the port.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var sourceDeviceType: AVCaptureDevice.DeviceType? { get }
```

## Discussion

All ports contained in an input’s ports property have the same source device type, which each equal to the deviceType property of the input’s device.

When working with virtual devices such as the builtInDualCamera in an AVCaptureMultiCamSession, it’s possible to stream media from the virtual device’s constituent device streams by discovering and connecting hidden ports. In the case of the builtInDualCamera, its constituent devices are the wide-angle and telephoto cameras.

By calling ports(for:sourceDeviceType:sourceDevicePosition:):, you may discover ports originating from one or more of the virtual device’s constituent devices and then make connections using those ports. Constituent device ports are never present in their owning virtual device input’s ports array.

## See Also

### Inspecting an Input Port

var isEnabled: Bool

A Boolean value that indicates whether the port is in an enabled state.

var mediaType: AVMediaType

The media type of the port.

var formatDescription: CMFormatDescription?

A description of the port format.

var sourceDevicePosition: AVCaptureDevice.Position

The position of the source device providing input through this port.

var clock: CMClock?

An object that represents the capture device’s clock.

