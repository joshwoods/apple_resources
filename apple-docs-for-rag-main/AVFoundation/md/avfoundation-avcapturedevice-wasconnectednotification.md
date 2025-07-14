

- AVFoundation
- AVCaptureDevice
-  wasConnectedNotification 

Type Property

# wasConnectedNotification

A notification the system posts when a new capture device becomes available.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 2.1+

``` source
class let wasConnectedNotification: NSNotification.Name
```

## Discussion

The notification’s object property contains the capture device that connected.

## See Also

### Finding and Monitoring Devices

class DiscoverySession

An object that finds capture devices that match specific search criteria.

class func `default`(AVCaptureDevice.DeviceType, for: AVMediaType?, position: AVCaptureDevice.Position) -> AVCaptureDevice?

Returns the default device for the specified device type, media type, and position.

class func `default`(for: AVMediaType) -> AVCaptureDevice?

Returns the default device that captures the specified media type.

init?(uniqueID: String)

Creates an object that represents a device with the specified identifier.

class let wasDisconnectedNotification: NSNotification.Name

A notification the system posts when an existing device becomes unavailable.

class func devices(for: AVMediaType) -> [AVCaptureDevice]

Returns devices capable of capturing media of the specified type.

Deprecated

class func devices() -> [AVCaptureDevice]

Returns all available capture devices on the system.

Deprecated

