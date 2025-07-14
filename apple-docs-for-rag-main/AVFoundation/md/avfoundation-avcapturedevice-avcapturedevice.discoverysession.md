

- AVFoundation
- AVCaptureDevice
-  AVCaptureDevice.DiscoverySession 

Class

# AVCaptureDevice.DiscoverySession

An object that finds capture devices that match specific search criteria.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+visionOS 2.1+

``` source
class DiscoverySession
```

## Mentioned in 

Choosing a Capture Device

## Overview

After creating a device discovery session, query its devices property to find a device to use for capture. You can also key-value observe this property to monitor changes to the list of available devices.

## Topics

### Creating a Session

convenience init(deviceTypes: [AVCaptureDevice.DeviceType], mediaType: AVMediaType?, position: AVCaptureDevice.Position)

Creates a discovery session that finds devices that match the specified criteria.

### Finding Devices

var devices: [AVCaptureDevice]

A list of devices that match the search criteria of the discovery session.

var supportedMultiCamDeviceSets: [Set&lt;AVCaptureDevice>]

Sets of capture devices that you can use simultaneously in a multi-camera session.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Finding and Monitoring Devices

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

class func devices() -> [AVCaptureDevice]

Returns all available capture devices on the system.

Deprecated

