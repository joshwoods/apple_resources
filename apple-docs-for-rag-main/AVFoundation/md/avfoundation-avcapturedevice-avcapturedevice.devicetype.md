

- AVFoundation
- AVCaptureDevice
-  AVCaptureDevice.DeviceType 

Structure

# AVCaptureDevice.DeviceType

A structure that defines the device types the framework supports.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+visionOS 2.1+

``` source
struct DeviceType
```

## Discussion

Use the device type constants to retrieve devices using an AVCaptureDevice.DiscoverySession object, or when calling the default(_:for:position:) method.

## Topics

### Cameras

static let builtInWideAngleCamera: AVCaptureDevice.DeviceType

A built-in wide-angle camera device type.

static let builtInUltraWideCamera: AVCaptureDevice.DeviceType

A built-in camera device type with a shorter focal length than a wide-angle camera.

static let builtInTelephotoCamera: AVCaptureDevice.DeviceType

A built-in camera device type with a longer focal length than a wide-angle camera.

static let builtInDualCamera: AVCaptureDevice.DeviceType

A built-in camera device type that consists of a wide-angle and telephoto camera.

static let builtInDualWideCamera: AVCaptureDevice.DeviceType

A built-in camera device type that consists of two cameras of fixed focal length, one ultrawide angle and one wide angle.

static let builtInTripleCamera: AVCaptureDevice.DeviceType

A built-in camera device type that consists of three cameras of fixed focal length, one ultrawide angle, one wide angle, and one telephoto.

static let continuityCamera: AVCaptureDevice.DeviceType

A Continuity Camera device type.

static let builtInDuoCamera: AVCaptureDevice.DeviceType

A built-in dual camera device type.

Deprecated

### Microphones

static let microphone: AVCaptureDevice.DeviceType

A microphone device type.

static let builtInMicrophone: AVCaptureDevice.DeviceType

A built-in microphone.

Deprecated

### External Devices

static let external: AVCaptureDevice.DeviceType

An external device type.

static let externalUnknown: AVCaptureDevice.DeviceType

An unknown external device type.

Deprecated

### Desk View

static let deskViewCamera: AVCaptureDevice.DeviceType

A virtual overhead camera that captures a user’s desk.

### Depth Sensing

static let builtInLiDARDepthCamera: AVCaptureDevice.DeviceType

A device that consists of two cameras, one LiDAR and one YUV.

static let builtInTrueDepthCamera: AVCaptureDevice.DeviceType

A device that consists of two cameras, one Infrared and one YUV.

### Initializers

init(rawValue: String)

Creates a capture device type with a string value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Identifying a Device

var uniqueID: String

An identifier that uniquely identifies the device.

var modelID: String

A model identifier for the device.

var localizedName: String

A localized device name for display in the user interface.

var manufacturer: String

A human-readable string for the manufacturer of the device.

var deviceType: AVCaptureDevice.DeviceType

The type of device, such as a built-in microphone or wide-angle camera.

var position: AVCaptureDevice.Position

The physical position of the capture device hardware.

enum Position

Constants that indicate the physical position of a capture device.

