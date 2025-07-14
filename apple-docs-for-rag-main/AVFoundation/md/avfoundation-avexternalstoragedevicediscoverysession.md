

- AVFoundation
-  AVExternalStorageDeviceDiscoverySession 

Class

# AVExternalStorageDeviceDiscoverySession

Informs your app when the external storage devices connect to and disconnect from the system.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
class AVExternalStorageDeviceDiscoverySession
```

## Topics

### Checking for session support on a device

class var isSupported: Bool

A Boolean value that indicates whether the system supports external storage devices.

### Retrieving the shared device discovery session instance

class var shared: AVExternalStorageDeviceDiscoverySession?

The system’s singleton device discovery session instance.

### Monitoring for storage device updates

var externalStorageDevices: [AVExternalStorageDevice]

An array of external storage devices the session updates as individual devices connect or disconnect from the system.

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

class AVExternalStorageDevice

Represents a physical external storage device that stores media assets.

