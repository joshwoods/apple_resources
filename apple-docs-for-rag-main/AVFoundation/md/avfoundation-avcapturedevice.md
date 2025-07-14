

- AVFoundation
-  AVCaptureDevice 

Class

# AVCaptureDevice

An object that represents a hardware or virtual capture device like a camera or microphone.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
class AVCaptureDevice
```

## Mentioned in 

Setting Up a Capture Session

Enhancing your app experience with the Camera Control

Choosing a Capture Device

Requesting authorization to capture and save media

## Overview

Capture devices provide media data to capture session inputs that you connect to an AVCaptureSession. An individual device can provide one or more streams of media of a particular type.

You don’t create capture device instances directly. Instead, retrieve them using an instance of AVCaptureDevice.DiscoverySession, or by calling the default(_:for:position:) method.

A capture device provides several configuration options. Before attempting to configure device properties, such as its focus mode, exposure mode, and so on, you must first acquire a lock on the device by calling the lockForConfiguration() method. You should also query the device’s capabilities to ensure that the new modes you intend to set are valid for the device. You can then set the properties and release the lock using the unlockForConfiguration() method. You may hold the lock if you want all settable device properties to remain unchanged. However, holding the device lock unnecessarily may degrade capture quality in other apps sharing the device and isn’t recommended.

## Topics

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

class func devices() -> [AVCaptureDevice]

Returns all available capture devices on the system.

Deprecated

### Authorizing Device Access

class func requestAccess(for: AVMediaType, completionHandler: (Bool) -> Void)

Requests the user’s permission to allow the app to capture media of a particular type.

class func authorizationStatus(for: AVMediaType) -> AVAuthorizationStatus

Returns an authorization status that indicates whether the user grants the app permission to capture media of a particular type.

enum AVAuthorizationStatus

Constants that indicate the status of an app’s authorization to capture media.

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

struct DeviceType

A structure that defines the device types the framework supports.

var position: AVCaptureDevice.Position

The physical position of the capture device hardware.

enum Position

Constants that indicate the physical position of a capture device.

### Accessing Device State

var isConnected: Bool

A Boolean value that indicates whether a device is currently connected to the system and available for use.

var isSuspended: Bool

A Boolean value that indicates whether the device is in a suspended state.

var isInUseByAnotherApplication: Bool

A Boolean value that indicates whether another app is using the device.

### Inspecting Device Characteristics

var isVirtualDevice: Bool

A Boolean value that indicates whether the device consists of two or more physical devices.

var constituentDevices: [AVCaptureDevice]

An array of physical devices that make up a virtual device.

func hasMediaType(AVMediaType) -> Bool

Returns a Boolean value that indicates whether the device captures media of a particular type.

var transportType: Int32

The transport type of the device.

func supportsSessionPreset(AVCaptureSession.Preset) -> Bool

Returns a Boolean value that indicates whether you can use the device with capture session configured with the specified preset.

### Monitoring Device Rotation

class RotationCoordinator

A class that monitors the physical orientation of a capture device and provides adjustment angles to keep images level, relative to gravity.

### Configuring Camera Hardware

func lockForConfiguration() throws

Requests exclusive access to configure device hardware properties.

func unlockForConfiguration()

Releases exclusive control over device hardware properties.

var isSubjectAreaChangeMonitoringEnabled: Bool

A Boolean value that indicates whether the device monitors the subject area for changes.

class let subjectAreaDidChangeNotification: NSNotification.Name

A notification the system posts when a capture device detects a substantial change to the video subject area.

Formats

Configure capture formats and camera frame rates.

Focus

Configure the automatic focus behavior of a camera, or manually set its lens position.

Exposure

Configure the automatic exposure behavior of a camera, or manually control its exposure settings.

White Balance

Configure the automatic white balance behavior of a camera, or manually control white balance settings.

Lighting

Configure the device flash, torch, and low light settings.

Color

Manage HDR and color space settings for a device.

Zoom

Configure device zooming behavior and inspect hardware capabilities.

### Enabling Automatic Frame Rate

var isAutoVideoFrameRateEnabled: Bool

A Boolean value that indicates whether the capture device performs automatic video frame rate adjustments.

### Supporting Spatial Capture

var spatialCaptureDiscomfortReasons: Set&lt;AVSpatialCaptureDiscomfortReason>

Reasons why current environmental conditions aren’t suitable to capturing spatial videos that are comfortable to view.

struct AVSpatialCaptureDiscomfortReason

Constants that indicate the suitability of the current scene to create a comfortable viewing experience.

### Supporting Continuity Camera

class var systemPreferredCamera: AVCaptureDevice?

A camera the system prefers to use for video and photo capture.

class var userPreferredCamera: AVCaptureDevice?

A camera the user prefers to use for video and photo capture.

var isContinuityCamera: Bool

A Boolean value that indicates whether the device is a Continuity Camera.

var companionDeskViewCamera: AVCaptureDevice?

A Desk View camera associated with a device.

### Supporting System Features

System Video Effects and Microphone Modes

Configure the state of system video effects like Center Stage, and inspect enhancements the system applies to microphone audio.

### Monitoring System Pressure

var systemPressureState: AVCaptureDevice.SystemPressureState

A value that indicates the capture device’s current system pressure state.

class SystemPressureState

An object that provides information about OS and hardware status affecting capture system performance and availability.

let AVCaptureSessionInterruptionSystemPressureStateKey: String

A key to retrieve a state value that indicates the system pressure level and contributing factors that caused the interruption.

### Restricting Camera Switching

func setPrimaryConstituentDeviceSwitchingBehavior(AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior, restrictedSwitchingBehaviorConditions: AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions)

Sets the switching behavior of the primary constituent device.

var primaryConstituentDeviceSwitchingBehavior: AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior

The switching behavior for the primary constituent device.

var primaryConstituentDeviceRestrictedSwitchingBehaviorConditions: AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions

The conditions that restrict the primary constituent device’s switching behavior.

var activePrimaryConstituentDeviceSwitchingBehavior: AVCaptureDevice.PrimaryConstituentDeviceSwitchingBehavior

The switching behavior of the active constituent device.

var activePrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions: AVCaptureDevice.PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions

The conditions that restrict camera switching behavior for the active primary constituent device.

var activePrimaryConstituent: AVCaptureDevice?

A virtual device’s active primary constituent device.

enum PrimaryConstituentDeviceSwitchingBehavior

Constants that control when to allow a virtual device to switch its active primary constituent device.

struct PrimaryConstituentDeviceRestrictedSwitchingBehaviorConditions

A structure that defines the conditions in which to restrict camera switching.

var supportedFallbackPrimaryConstituentDevices: [AVCaptureDevice]

The constituent devices available to select as a fallback for a longer focal length primary constituent device.

var fallbackPrimaryConstituentDevices: [AVCaptureDevice]

The fallback devices to use when a constituent device with a longer focal length becomes limited by its light sensitivity or minimum focus distance.

### Configuring macOS Features

macOS Capture Features

Control the transport behavior and input sources of capture hardware in macOS.

### Accessing Camera Extrinsics

class func extrinsicMatrix(from: AVCaptureDevice, to: AVCaptureDevice) -> Data?

Returns the relative extrinsic matrix from one capture device to another.

### Determining Lens Stabilization

enum LensStabilizationStatus

Constants that indicate the status of optical image stabilization hardware during a bracketed photo capture.

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

class AVCaptureDeviceInput

An object that provides media input from a capture device to a capture session.

class AVContinuityDevice

A class that represents a physical iOS device that’s nearby and can provide access to its cameras and microphones.

class AVExternalStorageDevice

Represents a physical external storage device that stores media assets.

class AVExternalStorageDeviceDiscoverySession

Informs your app when the external storage devices connect to and disconnect from the system.

