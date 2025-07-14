

- AVFoundation
- AVCaptureInput
- AVCaptureInput.Port
-  formatDescription 

Instance Property

# formatDescription

A description of the port format.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
var formatDescription: CMFormatDescription? { get }
```

## Discussion

A format description object describes the format of the media the port currently provides. To observe changes to a port’s format, observe notifications of type formatDescriptionDidChangeNotification.

## See Also

### Inspecting an Input Port

var isEnabled: Bool

A Boolean value that indicates whether the port is in an enabled state.

var mediaType: AVMediaType

The media type of the port.

var sourceDeviceType: AVCaptureDevice.DeviceType?

The device type of the source camera that provides data to the port.

var sourceDevicePosition: AVCaptureDevice.Position

The position of the source device providing input through this port.

var clock: CMClock?

An object that represents the capture device’s clock.

