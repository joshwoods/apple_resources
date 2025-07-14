

- AVFoundation
- AVCaptureDevice
-  constituentDevices 

Instance Property

# constituentDevices

An array of physical devices that make up a virtual device.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var constituentDevices: [AVCaptureDevice] { get }
```

## Discussion

The value of this property is an empty array when called on a device whose isVirtualDevice property is false.

## See Also

### Inspecting Device Characteristics

var isVirtualDevice: Bool

A Boolean value that indicates whether the device consists of two or more physical devices.

func hasMediaType(AVMediaType) -> Bool

Returns a Boolean value that indicates whether the device captures media of a particular type.

var transportType: Int32

The transport type of the device.

func supportsSessionPreset(AVCaptureSession.Preset) -> Bool

Returns a Boolean value that indicates whether you can use the device with capture session configured with the specified preset.

