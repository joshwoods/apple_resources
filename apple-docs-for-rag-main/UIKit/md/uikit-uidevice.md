

- UIKit
-  UIDevice 

Class

# UIDevice

A representation of the current device.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIDevice
```

## Overview

Use a UIDevice object to get information about the device such as assigned name, device model, and operating-system name and version. You also use the `UIDevice` instance to detect changes in the device’s characteristics, such as physical orientation. You get the current orientation using the orientation property or receive change notifications by registering for the orientationDidChangeNotification notification. Before using either of these techniques to get orientation data, you must enable data delivery using the beginGeneratingDeviceOrientationNotifications() method. When you no longer need to track the device orientation, call the endGeneratingDeviceOrientationNotifications() method to disable the delivery of notifications.

Similarly, you can use the `UIDevice` instance to obtain information and notifications about changes to the battery’s charge state (described by the batteryState property) and charge level (described by the batteryLevel property). The `UIDevice` instance also provides access to the proximity sensor state (described by the proximityState property). The proximity sensor detects whether the user is holding the device close to their face. Enable battery monitoring or proximity sensing only when you need it.

You can also use the playInputClick() instance method to play keyboard input clicks in custom input and keyboard accessory views.

## Topics

### Getting the shared device instance

class var current: UIDevice

An object that represents the current device.

### Identifying the device and operating system

var name: String

The name of the device.

var systemName: String

The name of the operating system running on the device.

var systemVersion: String

The current version of the operating system.

var model: String

The model of the device.

var localizedModel: String

The model of the device as a localized string.

var userInterfaceIdiom: UIUserInterfaceIdiom

The style of interface to use on the current device.

var identifierForVendor: UUID?

An alphanumeric string that uniquely identifies a device to the app’s vendor.

### Determining the available features

var isMultitaskingSupported: Bool

A Boolean value that indicates whether the current device supports multitasking.

### Tracking the device orientation

var orientation: UIDeviceOrientation

The physical orientation of the device.

enum UIDeviceOrientation

Constants that describe the physical orientation of the device.

var isGeneratingDeviceOrientationNotifications: Bool

A Boolean value that indicates whether the device generates orientation notifications.

func beginGeneratingDeviceOrientationNotifications()

Begins the generation of notifications of device orientation changes.

func endGeneratingDeviceOrientationNotifications()

Ends the generation of notifications of device orientation changes.

### Determining the current orientation

var isPortrait: Bool

A Boolean value that indicates whether the device is in a portrait orientation.

var isLandscape: Bool

A Boolean value that indicates whether the device is in a landscape orientation.

var isFlat: Bool

A Boolean value that indicates whether the specified orientation is face up or face down.

var isValidInterfaceOrientation: Bool

A Boolean value that indicates whether the specified orientation is one of the portrait or landscape orientations.

### Getting the device battery state

var batteryLevel: Float

The battery charge level for the device.

var isBatteryMonitoringEnabled: Bool

A Boolean value that indicates whether battery monitoring is enabled.

var batteryState: UIDevice.BatteryState

The battery state for the device.

enum BatteryState

Constants that describe the battery power state of the device.

### Using the proximity sensor

var isProximityMonitoringEnabled: Bool

A Boolean value that indicates whether proximity monitoring is enabled.

var proximityState: Bool

A Boolean value that indicates whether the proximity sensor is close to the user.

### Playing input clicks

func playInputClick()

Plays an input click in an enabled input view.

### Getting the current idiom

enum UIUserInterfaceIdiom

Constants that indicate the interface type for the device or an object that has a trait environment, such as a view and view controller.

func UI_USER_INTERFACE_IDIOM() -> UIUserInterfaceIdiom

Returns the interface idiom supported by the current device (recommended for apps that run in versions of iOS earlier than 3.2).

Deprecated

### Managing notifications

All UIDevice notifications are posted by the singleton device instance returned by current.

class let batteryLevelDidChangeNotification: NSNotification.Name

A notification that posts when the battery level changes.

class let batteryStateDidChangeNotification: NSNotification.Name

A notification that posts when battery state changes.

class let orientationDidChangeNotification: NSNotification.Name

A notification that posts when the orientation of the device changes.

class let proximityStateDidChangeNotification: NSNotification.Name

A notification that posts when the state of the proximity sensor changes.

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
- Sendable

## See Also

### Device environment

class UIStatusBarManager

An object that describes the configuration of the status bar.

