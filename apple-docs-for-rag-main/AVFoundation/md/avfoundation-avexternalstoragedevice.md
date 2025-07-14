

- AVFoundation
-  AVExternalStorageDevice 

Class

# AVExternalStorageDevice

Represents a physical external storage device that stores media assets.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
class AVExternalStorageDevice
```

## Overview

Each storage device instance corresponds to a physical external storage device where the system can media assets. You can access all of the currently available external storage devices with the AVExternalStorageDeviceDiscoverySession object’s externalStorageDevices property.

## Topics

### Checking permission to generate URLs

class var authorizationStatus: AVAuthorizationStatus

Your app’s authorization status for the external storage device.

### Requesting permission to generate URLs

class func requestAccess(completionHandler: (Bool) -> Void)

Requests access to an external storage device on behalf of your app, which can present a dialog to a person on their device’s display.

### Generating URLs for image assets

func nextAvailableURLs(withPathExtensions: [String]) throws -> [URL]

Generates an array of security scoped URLs that are compliant for digital camera formats, where each element has a different path extension.

### Inspecting a storage device

var isConnected: Bool

A Boolean value that indicates whether the system has a connection to the external storage device.

var displayName: String?

The name of an external storage device that’s appropriate for a user interface.

var uuid: UUID?

The external storage device’s unique identifier.

var freeSize: Int

The amount of free storage space, in bytes, that’s available on the external storage device.

var totalSize: Int

The total amount of storage space, in bytes, that’s available on the external storage device.

var isNotRecommendedForCaptureUse: Bool

A Boolean value that indicates whether the external storage device is suitable for camera capture.

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

### Capture devices

Choosing a Capture Device

Select the front or back camera, or use advanced features like the TrueDepth camera or dual camera.

class AVCaptureDevice

An object that represents a hardware or virtual capture device like a camera or microphone.

class AVCaptureDeviceInput

An object that provides media input from a capture device to a capture session.

class AVContinuityDevice

A class that represents a physical iOS device that’s nearby and can provide access to its cameras and microphones.

class AVExternalStorageDeviceDiscoverySession

Informs your app when the external storage devices connect to and disconnect from the system.

