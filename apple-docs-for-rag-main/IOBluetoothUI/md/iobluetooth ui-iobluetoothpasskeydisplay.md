

- IOBluetooth UI
-  IOBluetoothPasskeyDisplay 

Class

# IOBluetoothPasskeyDisplay

macOS 10.2+

``` source
@MainActor
class IOBluetoothPasskeyDisplay
```

## Topics

### Instance Properties

var backgroundImageConstraint: NSLayoutConstraint!

var centeredView: NSView!

var isIncomingRequest: Bool

var passkey: String!

var returnHighlightImage: NSImage!

var returnImage: NSImage!

var usePasskeyNotificaitons: Bool

### Instance Methods

func advancePasskeyIndicator()

func resetPasskeyIndicator()

func retreatPasskeyIndicator()

func setPasskey(String!, for: IOBluetoothDevice!, usingSSP: Bool)

### Type Methods

class func sharedDisplayView() -> IOBluetoothPasskeyDisplay!

## Relationships

### Inherits From

- NSView

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
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

class IOBluetoothServiceBrowserController

A NSWindowController subclass to display a window to search for and perform SDP queries on bluetooth devices within range.

class IOBluetoothServiceBrowserControllerRef

