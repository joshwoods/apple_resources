

- IOBluetooth
-  IOBluetoothSDPServiceAttribute 

Class

# IOBluetoothSDPServiceAttribute

IOBluetoothSDPServiceAttribute represents a single SDP service attribute.

macOS

``` source
class IOBluetoothSDPServiceAttribute
```

## Overview

A service attribute contains two components: an attribute ID and a data element.

## Topics

### Initializers

init!(id: BluetoothSDPServiceAttributeID, attributeElement: IOBluetoothSDPDataElement!)

Initializes a new service attribute with the given ID and data element.

init!(id: BluetoothSDPServiceAttributeID, attributeElementValue: NSObject!)

Initializes a new service attribute with the given ID and element value.

### Instance Methods

func getDataElement() -> IOBluetoothSDPDataElement!

Returns the data element for the target service attribute.

func getID() -> BluetoothSDPServiceAttributeID

Returns the attribute ID for the target service attribute.

func getIDDataElement() -> IOBluetoothSDPDataElement!

Returns the data element representing the attribute ID for the target service attribute.

### Type Methods

class func withID(BluetoothSDPServiceAttributeID, attributeElement: IOBluetoothSDPDataElement!) -> Self!

Creates a new service attribute with the given ID and data element.

class func withID(BluetoothSDPServiceAttributeID, attributeElementValue: NSObject!) -> Self!

Creates a new service attribute with the given ID and element value.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

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

class IOBluetoothRFCOMMChannel

An instance of this class represents an RFCOMM channel as defined by the Bluetooth SDP spec..

class IOBluetoothRFCOMMChannelRef

