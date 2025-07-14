

- AVFoundation
- AVCaptureDevice
-  transportType 

Instance Property

# transportType

The transport type of the device.

macOS 10.7+

``` source
var transportType: Int32 { get }
```

## Discussion

The value of this property represents a capture device’s transport type, such as USB or PCI. The value is an IOKit framework transport type constant (`kIOAudioDeviceTransportType`).

## See Also

### Inspecting Device Characteristics

var isVirtualDevice: Bool

A Boolean value that indicates whether the device consists of two or more physical devices.

var constituentDevices: [AVCaptureDevice]

An array of physical devices that make up a virtual device.

func hasMediaType(AVMediaType) -> Bool

Returns a Boolean value that indicates whether the device captures media of a particular type.

func supportsSessionPreset(AVCaptureSession.Preset) -> Bool

Returns a Boolean value that indicates whether you can use the device with capture session configured with the specified preset.

