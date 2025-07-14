

- AVFoundation
- AVCaptureDevice
-  supportsSessionPreset(\_:) 

Instance Method

# supportsSessionPreset(\_:)

Returns a Boolean value that indicates whether you can use the device with capture session configured with the specified preset.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
func supportsSessionPreset(_ preset: AVCaptureSession.Preset) -> Bool
```

## Parameters 

`preset`  

A capture session preset.

## Return Value

true if you can use the device; otherwise, false.

## See Also

### Inspecting Device Characteristics

var isVirtualDevice: Bool

A Boolean value that indicates whether the device consists of two or more physical devices.

var constituentDevices: [AVCaptureDevice]

An array of physical devices that make up a virtual device.

func hasMediaType(AVMediaType) -> Bool

Returns a Boolean value that indicates whether the device captures media of a particular type.

var transportType: Int32

The transport type of the device.

