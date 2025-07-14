

- IOBluetooth UI
-  IOBluetoothPairingController 

Class

# IOBluetoothPairingController

A NSWindowController subclass to display a window to initiate pairing to other bluetooth devices.

macOS 10.2+

``` source
@MainActor
class IOBluetoothPairingController
```

## Overview

Implementation of a window controller to handle pairing with a bluetooth device. This class will handle connecting to the Bluetooth Daemon for the purposes of searches, and displaying the results. When necessary this class will display a sheet asking the user for a PIN code. This window will not return anything to the caller if it is canceled or if pairing occurs.

## Topics

### Instance Methods

func addAllowedUUID(IOBluetoothSDPUUID!)

Adds a UUID to the list of UUIDs that are used to validate the user’s selection.

func addAllowedUUIDArray([Any]!)

Adds an array of UUIDs to the list of UUIDs that are used to validate the user’s selection.

func clearAllowedUUIDs()

Resets the controller back to the default state where it will accept any device the user selects.

func getDescriptionText() -> String!

Returns the description text that appears in the device selector panel.

func getOptions() -> IOBluetoothServiceBrowserControllerOptions

Returns the option bits that control the panel’s behavior.

func getPrompt() -> String!

Returns the title of the default/select button in the device selector panel.

func getResults() -> [Any]!

Returns an NSArray of the devices that were paired.

func getSearchAttributes() -> UnsafePointer&lt;IOBluetoothDeviceSearchAttributes>!

Returns the search attributes that control the panel’s search/inquiry behavior.

func getTitle() -> String!

Returns the title of the device selector panel.

func runModal() -> Int32

Runs the pairing panel in a modal session to allow the user to select a Bluetooth device.

func setDescriptionText(String!)

Sets the description text that appears in the device selector panel.

func setOptions(IOBluetoothServiceBrowserControllerOptions)

Sets the option bits that control the panel’s behavior.

func setPrompt(String!)

Sets the title of the default/select button in the device selector panel.

func setSearchAttributes(UnsafePointer&lt;IOBluetoothDeviceSearchAttributes>!)

Sets the search attributes that control the panel’s search/inquiry behavior.

func setTitle(String!)

Sets the title of the panel when not run as a sheet.

## Relationships

### Inherits From

- NSWindowController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSeguePerforming
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- Sendable

## See Also

### Classes

class IOBluetoothAccessibilityIgnoredImageCell

class IOBluetoothAccessibilityIgnoredTextFieldCell

class IOBluetoothDeviceSelectorController

A NSWindowController subclass to display a window to initiate pairing to other bluetooth devices.

class IOBluetoothDeviceSelectorControllerRef

class IOBluetoothObjectPushUIController

An NSWindowController subclass that supports the creation of an IOBluetoothObjectPushUIController object.

class IOBluetoothPairingControllerRef

class IOBluetoothPasskeyDisplay

class IOBluetoothServiceBrowserController

A NSWindowController subclass to display a window to search for and perform SDP queries on bluetooth devices within range.

class IOBluetoothServiceBrowserControllerRef

