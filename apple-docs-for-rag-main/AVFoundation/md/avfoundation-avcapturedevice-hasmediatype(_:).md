

- AVFoundation
- AVCaptureDevice
-  hasMediaType(\_:) 

Instance Method

# hasMediaType(\_:)

Returns a Boolean value that indicates whether the device captures media of a particular type.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
func hasMediaType(_ mediaType: AVMediaType) -> Bool
```

## Parameters 

`mediaType`  

A media type, such as video, audio, or muxed.

## Return Value

true if the device captures media of the specified type; otherwise, false.

## See Also

### Inspecting Device Characteristics

var isVirtualDevice: Bool

A Boolean value that indicates whether the device consists of two or more physical devices.

var constituentDevices: [AVCaptureDevice]

An array of physical devices that make up a virtual device.

var transportType: Int32

The transport type of the device.

func supportsSessionPreset(AVCaptureSession.Preset) -> Bool

Returns a Boolean value that indicates whether you can use the device with capture session configured with the specified preset.

