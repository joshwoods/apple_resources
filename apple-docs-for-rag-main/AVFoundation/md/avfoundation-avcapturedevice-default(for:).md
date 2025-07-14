

- AVFoundation
- AVCaptureDevice
-  default(for:) 

Type Method

# default(for:)

Returns the default device that captures the specified media type.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 2.1+

``` source
class func `default`(for mediaType: AVMediaType) -> AVCaptureDevice?
```

## Parameters 

`mediaType`  

A media type for the device.

## Return Value

The default device, or `nil` if no device with that media type exists.

## See Also

### Finding and Monitoring Devices

class DiscoverySession

An object that finds capture devices that match specific search criteria.

class func `default`(AVCaptureDevice.DeviceType, for: AVMediaType?, position: AVCaptureDevice.Position) -> AVCaptureDevice?

Returns the default device for the specified device type, media type, and position.

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

