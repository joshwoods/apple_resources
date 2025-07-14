

- AVFoundation
- AVCaptureDevice
-  isVirtualDevice 

Instance Property

# isVirtualDevice

A Boolean value that indicates whether the device consists of two or more physical devices.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var isVirtualDevice: Bool { get }
```

## Discussion

Examples of virtual devices are:

- The dual camera, which supports seamless switching between wide-angle and telephoto cameras while zooming and generating depth data from the disparities between the points of view of the physical cameras.

- The TrueDepth camera, which generates depth data from disparities between YUV and infrared cameras pointed in the same direction.

## See Also

### Inspecting Device Characteristics

var constituentDevices: [AVCaptureDevice]

An array of physical devices that make up a virtual device.

func hasMediaType(AVMediaType) -> Bool

Returns a Boolean value that indicates whether the device captures media of a particular type.

var transportType: Int32

The transport type of the device.

func supportsSessionPreset(AVCaptureSession.Preset) -> Bool

Returns a Boolean value that indicates whether you can use the device with capture session configured with the specified preset.

