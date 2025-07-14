

- ImageCaptureCore
-  ICDevice 

Class

# ICDevice

An abstract object that represents a device.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
class ICDevice
```

## Overview

The device browser uses the concrete subclasses ICCameraDevice and ICScannerDevice to represent the cameras and scanners it finds.

## Topics

### Identifying a Device

var name: String?

The device’s name as reported by the device module, or if no device module is in control of this device, by the device transport.

var productKind: String?

The device’s type.

var icon: CGImage?

The device’s icon image.

var uuidString: String?

A string representation of the device’s universally unique identifier (UUID).

var persistentIDString: String?

A string representation of the device’s persistent ID.

var serialNumberString: String?

The device’s serial number.

### Inspecting a Device’s Type and Location

var type: ICDeviceType

A combination of the device’s type and its location type.

enum ICDeviceType

The type of image capture device.

enum ICDeviceTypeMask

Masks for detecting different device types.

var locationDescription: String?

A nonlocalized location description for the device.

var modulePath: String

The file system path of the device module associated with this device.

var moduleVersion: String?

The bundle version of the device module associated with this device.

enum ICDeviceLocationType

The location of the image capture device.

enum ICDeviceLocationTypeMask

Masks for detecting different device locations.

struct ICDeviceLocationOptions

Options for the location of the image capture device.

var usbLocationID: Int32

The USB location that the device is occupying.

var usbProductID: Int32

The USB Product ID (PID) associated with the device.

var usbVendorID: Int32

The USB Vendor ID (VID) associated with the device.

### Inspecting a Device’s Transport Type

var transportType: String?

The hardware connection type the device is using.

struct ICDeviceTransport

The hardware connection types a device can use.

### Inspecting a Device’s Capabilities

var capabilities: [String]

The capabilities of the device as reported by the device module.

struct ICDeviceCapability

Constants that describe the capabilities of a camera.

struct ICSessionOptions

Session options for altering the delivery of the device contents.

### Subscribing to Device Status Notifications

struct ICDeviceStatus

The status types that a device might deliver while in use.

### Managing a Device

var delegate: (any ICDeviceDelegate)?

The delegate to receive messages once a session is opened on the device.

protocol ICDeviceDelegate

Methods for responding to device events and changes.

var hasOpenSession: Bool

A Boolean value that indicates whether the device has an open session.

func requestOpenSession()

Requests to open a session on the device.

func requestOpenSession(options: [ICSessionOptions : Any]?, completion: ((any Error)?) -> Void)

Requests to open a session on the device, then executes the completion handler.

func requestSendMessage(UInt32, outData: Data, maxReturnedDataSize: UInt32, sendMessageDelegate: Any, didSendMessageSelector: Selector, contextInfo: UnsafeMutableRawPointer?)

Asynchronously sends an arbitrary message with optional data to a device.

func requestCloseSession()

Requests to close an open session on the device.

func requestCloseSession(options: [ICSessionOptions : Any]?, completion: ((any Error)?) -> Void)

Requests to close an open session on the device, then executes the completion handler.

func requestEject()

Requests to eject the media if permitted by the device, or to disconnect from a remote device.

func requestEject(completion: ((any Error)?) -> Void)

Requests to eject the media if permitted by the device, or to disconnect from a remote device, then executes the completion handler.

### Configuring a Device’s Characteristics

var userData: NSMutableDictionary?

A bookkeeping object for client convenience.

var autolaunchApplicationPath: String?

The file system path of an application to launch automatically when this device is added.

var isRemote: Bool

A Boolean value indicating whether the device is published by the Image Capture device-sharing facility.

### Deprecated Symbols

func requestEjectOrDisconnect()

Requests to eject the media if permitted by the device, or to disconnect from a remote device.

Deprecated

func requestYield()

Requests that device module in control of this device yield control.

Deprecated

var moduleExecutableArchitecture: Int32

The executable architecture of the device module servicing the requests.

Deprecated

### Instance Properties

var systemSymbolName: String?

## Relationships

### Inherits From

- NSObject

### Inherited By

- ICCameraDevice
- ICScannerDevice

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Browsing Devices

var isBrowsing: Bool

A Boolean value indicating whether the device browser is browsing for devices.

var devices: [ICDevice]?

All devices found by the browser.

var browsedDeviceTypeMask: ICDeviceTypeMask

A mask whose set bits indicate the type of devices being browsed after the delegate receives the start message.

func start()

Tells the delegate to start looking for devices.

func stop()

Tells the delegate to stop looking for devices.

