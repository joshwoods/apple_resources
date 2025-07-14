

- IOBluetooth UI
-  IOBluetoothServiceBrowserController 

Class

# IOBluetoothServiceBrowserController

A NSWindowController subclass to display a window to search for and perform SDP queries on bluetooth devices within range.

macOS 10.2+

``` source
@MainActor
class IOBluetoothServiceBrowserController
```

## Overview

This NSWindowController subclass will bring up a generic Bluetooth search and SDP browsing window allowing the user to find devices within range, perform SDP queries on a particular device, and select a SDP service to connect to. The client application can provide NSArrays of valid service UUIDs to allow, and an NSArray of valid device types to allow. The device type filter is not yet implemented.

## Topics

### Initializers

init!(IOBluetoothServiceBrowserControllerOptions)

Allocator work Bluetooth Service Browser window controller.

### Instance Methods

func addAllowedUUID(IOBluetoothSDPUUID!)

Adds a UUID to the list of UUIDs that are used to validate the user’s selection.

func addAllowedUUIDArray([Any]!)

Adds an array of UUIDs to the list of UUIDs that are used to validate the user’s selection.

func beginSheetModal(for: NSWindow!, modalDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!) -> IOReturn

Runs the service browser panel as a sheet on the target window.

func clearAllowedUUIDs()

Resets the controller back to the default state where it will accept any device the user selects.

func getDescriptionText() -> String!

Returns the description text that appears in the device selector panel.

func getOptions() -> IOBluetoothServiceBrowserControllerOptions

Returns the option bits that control the panel’s behavior.

func getPrompt() -> String!

Returns the title of the default/select button in the device selector panel.

func getRef() -> Unmanaged&lt;IOBluetoothServiceBrowserControllerRef>!

Returns an IOBluetoothServiceBrowserControllerRef representation of the target IOBluetoothServiceBrowserController object.

func getResults() -> [Any]!

Returns the result of the user’s selection.

func getSearchAttributes() -> UnsafePointer&lt;IOBluetoothDeviceSearchAttributes>!

Returns the search attributes that control the panel’s search/inquiry behavior.

func getTitle() -> String!

Returns the title of the device selector panel.

func runModal() -> Int32

Runs the service browser panel in a modal session to allow the user to select a service on a Bluetooth device.

func setDescriptionText(String!)

Sets the description text that appears in the device selector panel.

func setOptions(IOBluetoothServiceBrowserControllerOptions)

Modify the options for the window controller.

func setPrompt(String!)

Sets the title of the default/select button in the device selector panel.

func setSearchAttributes(UnsafePointer&lt;IOBluetoothDeviceSearchAttributes>!)

Sets the search attributes that control the panel’s search/inquiry behavior.

func setTitle(String!)

Sets the title of the panel when not run as a sheet.

### Type Methods

class func withServiceBrowserControllerRef(IOBluetoothServiceBrowserControllerRef!) -> IOBluetoothServiceBrowserController!

Method call to convert an IOBluetoothServiceBrowserControllerRef into an IOBluetoothServiceBrowserController \*.

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

class IOBluetoothPairingController

A NSWindowController subclass to display a window to initiate pairing to other bluetooth devices.

class IOBluetoothPairingControllerRef

class IOBluetoothPasskeyDisplay

class IOBluetoothServiceBrowserControllerRef

