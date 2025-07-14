

- IOBluetooth UI
-  IOBluetoothDeviceSelectorController 

Class

# IOBluetoothDeviceSelectorController

A NSWindowController subclass to display a window to initiate pairing to other bluetooth devices.

macOS 10.2+

``` source
@MainActor
class IOBluetoothDeviceSelectorController
```

## Overview

Implementation of a window controller to return a NSArray of selected bluetooth devices. This class will handle connecting to the Bluetooth Daemon for the purposes of searches, and displaying the results. This controller will return a NSArray of IOBluetoothDevice objects to the user.

## Topics

### Instance Methods

func addAllowedUUID(IOBluetoothSDPUUID!)

Adds a UUID to the list of UUIDs that are used to validate the user’s selection.

func addAllowedUUIDArray([Any]!)

Adds an array of UUIDs to the list of UUIDs that are used to validate the user’s selection.

func beginSheetModal(for: NSWindow!, modalDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!) -> IOReturn

Runs the device selector panel as a sheet on the target window.

func clearAllowedUUIDs()

Resets the controller back to the default state where it will accept any device the user selects.

func getCancel() -> String!

Returns the title of the default/cancel button in the device selector panel.

func getDescriptionText() -> String!

Returns the description text that appears in the device selector panel.

func getHeader() -> String!

Returns the header text that appears in the device selector panel.

func getOptions() -> IOBluetoothServiceBrowserControllerOptions

Returns the option bits that control the panel’s behavior.

func getPrompt() -> String!

Returns the title of the default/select button in the device selector panel.

func getResults() -> [Any]!

Returns the result of the user’s selection.

func getSearchAttributes() -> UnsafePointer&lt;IOBluetoothDeviceSearchAttributes>!

Returns the search attributes that control the panel’s search/inquiry behavior.

func getTitle() -> String!

Returns the title of the device selector panel.

func runModal() -> Int32

Runs the device selector panel in a modal session to allow the user to select a Bluetooth device.

func setCancel(String!)

Sets the title of the default/cancel button in the device selector panel.

func setDescriptionText(String!)

Sets the description text that appears in the device selector panel.

func setHeader(String!)

Sets the header text that appears in the device selector panel.

func setOptions(IOBluetoothServiceBrowserControllerOptions)

Sets the option bits that control the panel’s behavior.

func setPrompt(String!)

Sets the title of the default/select button in the device selector panel.

func setSearchAttributes(UnsafePointer&lt;IOBluetoothDeviceSearchAttributes>!)

Sets the search attributes that control the panel’s search/inquiry behavior.

func setTitle(String!)

Sets the title of the panel when not run as a sheet.

### Type Methods

class func deviceSelector() -> IOBluetoothDeviceSelectorController!

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

## See Also

### Classes

class IOBluetoothAccessibilityIgnoredImageCell

class IOBluetoothAccessibilityIgnoredTextFieldCell

class IOBluetoothDeviceSelectorControllerRef

class IOBluetoothObjectPushUIController

An NSWindowController subclass that supports the creation of an IOBluetoothObjectPushUIController object.

class IOBluetoothPairingController

A NSWindowController subclass to display a window to initiate pairing to other bluetooth devices.

class IOBluetoothPairingControllerRef

class IOBluetoothPasskeyDisplay

class IOBluetoothServiceBrowserController

A NSWindowController subclass to display a window to search for and perform SDP queries on bluetooth devices within range.

class IOBluetoothServiceBrowserControllerRef

