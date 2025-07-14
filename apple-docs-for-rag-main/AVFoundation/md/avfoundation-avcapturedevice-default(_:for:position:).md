

- AVFoundation
- AVCaptureDevice
-  default(\_:for:position:) 

Type Method

# default(\_:for:position:)

Returns the default device for the specified device type, media type, and position.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+visionOS 2.1+

``` source
class func `default`(
    _ deviceType: AVCaptureDevice.DeviceType,
    for mediaType: AVMediaType?,
    position: AVCaptureDevice.Position
) -> AVCaptureDevice?
```

## Parameters 

`deviceType`  

The type of capture device to request, such as builtInWideAngleCamera.

`mediaType`  

The type of media to request capture of, such as video or audio.

`position`  

The position of capture device to request relative to system hardware (front- or back-facing). Pass AVCaptureDevice.Position.unspecified to search for devices regardless of position.

## Return Value

The default system device, or `nil` if no device currently exists that satisfies the specified criteria.

## Mentioned in 

Choosing a Capture Device

## Discussion

Use this method to select the system default capture device for a given scenario. For example, to obtain the dual camera on supported hardware and fall back to the standard wide-angle camera otherwise, call this method twice, as shown below.

```
// The app's default camera.
var defaultCamera: AVCaptureDevice? {
    // Find the built-in dual camera, if it exists.
    if let device = AVCaptureDevice.default(.builtInDualCamera,
                                            for: .video,
                                            position: .back) {
        return device
    }

    // Find the built-in wide-angle camera, if it exists.
    if let device = AVCaptureDevice.default(.builtInWideAngleCamera,
                                            for: .video,
                                            position: .back) {
        return device
    }
    return nil
}
```

## See Also

### Finding and Monitoring Devices

class DiscoverySession

An object that finds capture devices that match specific search criteria.

class func `default`(for: AVMediaType) -> AVCaptureDevice?

Returns the default device that captures the specified media type.

init?(uniqueID: String)

Creates an object that represents a device with the specified identifier.

class let wasConnectedNotification: NSNotification.Name

A notification the system posts when a new capture device becomes available.

class let wasDisconnectedNotification: NSNotification.Name

A notification the system posts when an existing device becomes unavailable.

class func devices(for: AVMediaType) -> [AVCaptureDevice]

Returns devices capable of capturing media of the specified type.

Deprecated

class func devices() -> [AVCaptureDevice]

Returns all available capture devices on the system.

Deprecated

