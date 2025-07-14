

- AVFoundation
- AVCaptureDeviceInput
-  ports(for:sourceDeviceType:sourceDevicePosition:) 

Instance Method

# ports(for:sourceDeviceType:sourceDevicePosition:)

Retrieves a virtual device’s constituent device ports for use in a multi-camera session.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
func ports(
    for mediaType: AVMediaType?,
    sourceDeviceType: AVCaptureDevice.DeviceType?,
    sourceDevicePosition: AVCaptureDevice.Position
) -> [AVCaptureInput.Port]
```

## Parameters 

`mediaType`  

The media type of the port you’re searching for, or `nil` to consider all media types.

`sourceDeviceType`  

The device type of the port you’re searching for, or `nil` if to consider all device types.

`sourceDevicePosition`  

The device position of the port you’re searching for.

When you’re searching for a camera device, a position of AVCaptureDevice.Position.unspecified indicates to search for all positions.

When you’re searching for an audio device, AVCaptureDevice.Position.unspecified indicates to search omnidirectional audio.

## Return Value

An array of ports that satisfy the search criteria, or an empty array if there are none.

## Discussion

AVCaptureMultiCamSession lets you simultaneously capture from multiple devices. It also lets you capture simultaneous streams from a virtual device, such as the dual camera. You use this method to find the ports associated with a virtual device’s underlying physical devices. A virtual device input’s ports property doesn’t include constituent device ports.

Using the dual camera as an example, the ports property exposes only those ports supported by the virtual device (it switches automatically between wide-angle and telephoto cameras, depending on the zoom factor). You may use this method to find the video ports for the constituent devices.

```
// Look up the wide-angle camera port.
let wideVideoPort = dualCameraInput.ports(for: .video,
                                          sourceDeviceType: .builtInWideAngleCamera,
                                          sourceDevicePosition: .back).first

// Look up the telephoto camera port.
let teleVideoPort = dualCameraInput.ports(for: .video,
                                          sourceDeviceType: .builtInTelephotoCamera,
                                          sourceDevicePosition: .back).first
```

You can use these ports to create connections to two instances of AVCaptureVideoDataOutput, allowing for synchronized, full-frame-rate delivery of both wide-angle and telephoto streams.

When used in conjunction with an audio device, this method allows you to discover microphones in different positions. You can use the microphone ports to make output connections to simultaneously capture both front-facing and back-facing audio. The audio device port whose sourceDevicePosition is AVCaptureDevice.Position.unspecified produces omnidirectional sound.

## See Also

### Accessing the Device

var device: AVCaptureDevice

A capture device associated with this input.

