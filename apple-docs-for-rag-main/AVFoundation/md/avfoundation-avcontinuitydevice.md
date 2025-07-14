

- AVFoundation
-  AVContinuityDevice 

Class

# AVContinuityDevice

A class that represents a physical iOS device that’s nearby and can provide access to its cameras and microphones.

tvOS 17.0+

``` source
class AVContinuityDevice
```

## Overview

Each continuity device instance represents another iOS device that’s nearby. Your app can access the other device’s cameras and microphones with its videoDevices and audioSessionInputs properties, respectively.

## Topics

### Checking a continuity device’s availability

var isConnected: Bool

A Boolean value that indicates whether you can use the continuity device because it’s connected to the system.

### Retrieving video devices from a continuity device

var videoDevices: [AVCaptureDevice]

An array of the continuity device’s video-capture devices available to your app.

### Retrieving audio ports from a continuity device

var audioSessionInputs: [AVAudioSessionPortDescription]

An array of the continuity device’s audio session port descriptions that’s available to your app.

### Identifying a continuity device

var connectionID: UUID

A universally unique value that identifies a specific continuity device.

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

class AVExternalStorageDevice

Represents a physical external storage device that stores media assets.

class AVExternalStorageDeviceDiscoverySession

Informs your app when the external storage devices connect to and disconnect from the system.

