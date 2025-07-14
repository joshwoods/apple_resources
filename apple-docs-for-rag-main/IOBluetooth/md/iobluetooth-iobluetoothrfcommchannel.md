

- IOBluetooth
-  IOBluetoothRFCOMMChannel 

Class

# IOBluetoothRFCOMMChannel

An instance of this class represents an RFCOMM channel as defined by the Bluetooth SDP spec..

macOS

``` source
class IOBluetoothRFCOMMChannel
```

## Overview

An RFCOMM channel object can be obtained by opening an RFCOMM channel in a device, or by requesting a notification when a channel is created (this is commonly used to provide services).

## Topics

### Instance Methods

func close() -> IOReturn

Close the channel.

func delegate() -> Any!

Returns the object delegate

func getDevice() -> IOBluetoothDevice!

Returns the Bluetooth Device that carries the rfcomm data.

func getID() -> BluetoothRFCOMMChannelID

Returns the object rfcomm channel ID.

func getMTU() -> BluetoothRFCOMMMTU

Returns the channel maximum transfer unit.

func getObjectID() -> IOBluetoothObjectID

Returns the IOBluetoothObjectID of the given IOBluetoothRFCOMMChannel.

func getRef() -> Unmanaged&lt;IOBluetoothRFCOMMChannelRef>!

Returns an IOBluetoothRFCOMMChannelRef representation of the target IOBluetoothRFCOMMChannel object.

func isIncoming() -> Bool

Returns the direction of the channel. An incoming channel is one that was opened by the remote device.

func isOpen() -> Bool

Returns the state of the channel.

func isTransmissionPaused() -> Bool

Returns TRUE if flow control is off.

func register(forChannelCloseNotification: Any!, selector: Selector!) -> IOBluetoothUserNotification!

Allows a client to register for a channel close notification.

func sendRemoteLineStatus(BluetoothRFCOMMLineStatus) -> IOReturn

Sends an error to the remote side.

func setDelegate(Any!) -> IOReturn

Allows an object to register itself as a client of the RFCOMM channel.

func setSerialParameters(UInt32, dataBits: UInt8, parity: BluetoothRFCOMMParityType, stopBits: UInt8) -> IOReturn

Changes the parameters of the serial connection.

func writeAsync(UnsafeMutableRawPointer!, length: UInt16, refcon: UnsafeMutableRawPointer!) -> IOReturn

Sends a block of data in the channel asynchronously.

func writeSync(UnsafeMutableRawPointer!, length: UInt16) -> IOReturn

Sends a block of data in the channel synchronously.

### Type Methods

class func register(forChannelOpenNotifications: Any!, selector: Selector!) -> IOBluetoothUserNotification!

Allows a client to register for RFCOMM channel open notifications for any RFCOMM channel.

class func register(forChannelOpenNotifications: Any!, selector: Selector!, withChannelID: BluetoothRFCOMMChannelID, direction: IOBluetoothUserNotificationChannelDirection) -> IOBluetoothUserNotification!

Allows a client to register for RFCOMM channel open notifications for certain types of RFCOMM channels.

class func withObjectID(IOBluetoothObjectID) -> Self!

Returns the IObluetoothRFCOMMChannel with the given IOBluetoothObjectID.

class func withRFCOMMChannelRef(IOBluetoothRFCOMMChannelRef!) -> Self!

Method call to convert an IOBluetoothRFCOMMChannelRef into an IOBluetoothRFCOMMChannel \*.

## Relationships

### Inherits From

- IOBluetoothObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- PortDelegate
- StreamDelegate

## See Also

### Classes

class IOBluetoothDevice

An instance of IOBluetoothDevice represents a single remote Bluetooth device.

class IOBluetoothDeviceInquiry

Object representing a device inquiry that finds Bluetooth devices in-range of the computer, and (optionally) retrieves name information for them.

class IOBluetoothDevicePair

An instance of IOBluetoothDevicePair represents a pairing attempt to a remote Bluetooth device.

class IOBluetoothDeviceRef

An object that represents a Bluetooth I/O device.

class IOBluetoothHandsFree

Hands free profile class.

class IOBluetoothHandsFreeAudioGateway

An object that sends data to a connected Bluetooth hands-free phone or headset and processes commands from it.

class IOBluetoothHandsFreeDevice

An object you use to manage phone calls on a connected Bluetooth hands-free phone or headset.

class IOBluetoothHostController

This class is a representation of a Bluetooth Host Controller Interface that is present on the local computer (either plugged in externally or available internally).

class IOBluetoothL2CAPChannel

An instance of IOBluetoothL2CAPChannel represents a single open L2CAP channel.

class IOBluetoothL2CAPChannelRef

class IOBluetoothOBEXSession

An OBEX Session with a Bluetooth RFCOMM channel as the transport.

class IOBluetoothObject

class IOBluetoothObjectRef

class IOBluetoothRFCOMMChannelRef

class IOBluetoothSDPDataElement

An instance of this class represents a single SDP data element as defined by the Bluetooth SDP spec.

