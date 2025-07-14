

- External Accessory
-  EAAccessoryManager 

Class

# EAAccessoryManager

The object you use to identify connected accessories, and begin delivery of connection and disconnection notifications.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
class EAAccessoryManager
```

## Overview

An EAAccessoryManager object coordinates the attached accessories for an iOS-based device. Use the shared accessory manager to retrieve a list of connected accessories, and start and stop the delivery of connection and disconnection notifications.

Important

iPhone and iPad apps running on Macs with Apple silicon never receive connection notifications.

## Topics

### Getting the Shared Accessory Manager

class func shared() -> EAAccessoryManager

Returns the shared accessory manager object for the iOS-based device.

### Managing Connection Status Changes

func registerForLocalNotifications()

Begins the delivery of accessory-related notifications to the current application.

func unregisterForLocalNotifications()

Stops the delivery of accessory-related notifications to the current application.

static let EAAccessoryDidConnect: NSNotification.Name

A notification that the system sends when an accessory becomes connected and available for your application to use.

static let EAAccessoryDidDisconnect: NSNotification.Name

A notification that is posted when an accessory is disconnected and no longer available for your application to use.

let EAAccessoryKey: String

A key that indicates the accessory object whose status changed.

let EAAccessorySelectedKey: String

A key that indicates the accessory object that the user selected.

### Presenting the Bluetooth Picker

func showBluetoothAccessoryPicker(withNameFilter: NSPredicate?, completion: EABluetoothAccessoryPickerCompletion?)

Displays an alert that allows the user to pair the device with a Bluetooth accessory.

typealias EABluetoothAccessoryPickerCompletion

The completion block for the Bluetooth picker.

struct EABluetoothAccessoryPickerError

Error codes returned by the Bluetooth accessory picker.

enum Code

The error codes that may be passed in an error object for the Bluetooth picker completion block.

let EABluetoothAccessoryPickerErrorDomain: String

The domain for errors passed to a Bluetooth picker completion block.

### Getting the Available Accessories

var connectedAccessories: [EAAccessory]

The accessory objects corresponding to the list of currently connected accessories.

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

### Essentials

UISupportedExternalAccessoryProtocols

The protocols that the app uses to communicate with external accessory hardware.

