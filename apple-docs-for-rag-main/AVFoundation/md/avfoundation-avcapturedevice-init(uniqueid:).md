

- AVFoundation
- AVCaptureDevice
-  init(uniqueID:) 

Initializer

# init(uniqueID:)

Creates an object that represents a device with the specified identifier.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 2.1+

``` source
init?(uniqueID deviceUniqueID: String)
```

## Parameters 

`deviceUniqueID`  

An identifier that uniquely identifies the device.

## Return Value

A capture device, or `nil` if no device with the specified identifier exists.

## Discussion

Every capture device has a unique identifier that persists on a system across device connections, app restarts, and reboots of the system itself.

## See Also

### Finding and Monitoring Devices

class DiscoverySession

An object that finds capture devices that match specific search criteria.

class func `default`(AVCaptureDevice.DeviceType, for: AVMediaType?, position: AVCaptureDevice.Position) -> AVCaptureDevice?

Returns the default device for the specified device type, media type, and position.

class func `default`(for: AVMediaType) -> AVCaptureDevice?

Returns the default device that captures the specified media type.

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

