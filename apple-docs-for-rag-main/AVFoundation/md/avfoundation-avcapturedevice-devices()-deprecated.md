

- AVFoundation
- AVCaptureDevice
-  devices() Deprecated

Type Method

# devices()

Returns all available capture devices on the system.

iOS 4.0–10.0DeprecatediPadOS 4.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.7–10.15Deprecated

``` source
class func devices() -> [AVCaptureDevice]
```

Deprecated

Use the AVCaptureDevice.DiscoverySession class instead.

## Return Value

An array of available devices.

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

class let wasConnectedNotification: NSNotification.Name

A notification the system posts when a new capture device becomes available.

class let wasDisconnectedNotification: NSNotification.Name

A notification the system posts when an existing device becomes unavailable.

class func devices(for: AVMediaType) -> [AVCaptureDevice]

Returns devices capable of capturing media of the specified type.

Deprecated

