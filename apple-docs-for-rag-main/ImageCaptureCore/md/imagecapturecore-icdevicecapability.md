

- ImageCaptureCore
-  ICDeviceCapability 

Structure

# ICDeviceCapability

Constants that describe the capabilities of a camera.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
struct ICDeviceCapability
```

## Topics

### Creating Device Capabilities

init(rawValue: String)

Creates an ImageCaptureCore device capability.

### Taking Pictures

static let cameraDeviceCanTakePicture: ICDeviceCapability

The capability for the client to request to take a picture while the camera is connected.

static let cameraDeviceCanTakePictureUsingShutterReleaseOnCamera: ICDeviceCapability

The capability to capture a picture if the user presses the shutter release on the camera while the camera is connected.

### Deleting Files

static let cameraDeviceCanDeleteOneFile: ICDeviceCapability

Indicates that the camera can delete a file at a time while it is connected.

static let cameraDeviceCanDeleteAllFiles: ICDeviceCapability

Indicates that the camera can delete all files in a single operation while it is connected.

### Uploading Files

static let cameraDeviceCanReceiveFile: ICDeviceCapability

Indicates that the host can upload files to the camera.

### Synchronizing the Clock

static let cameraDeviceCanSyncClock: ICDeviceCapability

Indicates that the camera can synchronize its date and time with that of the host computer.

### Sending PTP Commands

static let cameraDeviceCanAcceptPTPCommands: ICDeviceCapability

Indicates that the camera can accept PTP commands.

### Disconnecting

static let canEjectOrDisconnect: ICDeviceCapability

Indicates that the camera can eject or disconnect.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting a Device’s Capabilities

var capabilities: [String]

The capabilities of the device as reported by the device module.

struct ICSessionOptions

Session options for altering the delivery of the device contents.

