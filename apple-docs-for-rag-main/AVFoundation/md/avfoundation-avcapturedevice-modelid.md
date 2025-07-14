

- AVFoundation
- AVCaptureDevice
-  modelID 

Instance Property

# modelID

A model identifier for the device.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 2.1+

``` source
var modelID: String { get }
```

## Discussion

The value of this property is an identifier unique to all devices of the same model. The value is persistent across device connections and disconnections, and across different systems. For example, the model identifier of a built-in camera on two identical iPhone models is the same even though they’re different physical devices.

## See Also

### Identifying a Device

var uniqueID: String

An identifier that uniquely identifies the device.

var localizedName: String

A localized device name for display in the user interface.

var manufacturer: String

A human-readable string for the manufacturer of the device.

var deviceType: AVCaptureDevice.DeviceType

The type of device, such as a built-in microphone or wide-angle camera.

struct DeviceType

A structure that defines the device types the framework supports.

var position: AVCaptureDevice.Position

The physical position of the capture device hardware.

enum Position

Constants that indicate the physical position of a capture device.

