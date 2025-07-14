

- IOBluetooth
-  IOBluetoothSDPUUID 

Class

# IOBluetoothSDPUUID

An NSData subclass that represents a UUID as defined in the Bluetooth SDP spec.

macOS

``` source
class IOBluetoothSDPUUID
```

## Overview

The IOBluetoothSDPUUID class can represent a UUID of any valid size (16, 32 or 128 bits). It provides the ability to compare two UUIDs no matter what their size as well as the ability to promote the size of a UUID to a larger one.

## Topics

### Initializers

convenience init!(bytes: UnsafeRawPointer!, length: UInt32)

Creates a new IOBluetoothSDPUUID object with the given bytes of the given length.

convenience init!(data: Data!)

Creates a new IOBluetoothSDPUUID object from the given NSData.

init!(uuid16: BluetoothSDPUUID16)

Initializes a new 16-bit IOBluetoothSDPUUID with the given UUID16

init!(uuid32: BluetoothSDPUUID32)

Creates a new 32-bit IOBluetoothSDPUUID with the given UUID32

### Instance Methods

func classForArchiver() -> AnyClass!

func classForCoder() -> AnyClass!

func classForPortCoder() -> AnyClass!

func getWithLength(UInt32) -> Self!

Returns an IOBluetoothSDPUUID object matching the target UUID, but with the given number of bytes.

func isEqual(to: IOBluetoothSDPUUID!) -> Bool

Compares the target IOBluetoothSDPUUID object with the given otherUUID object.

### Type Methods

class func uuid16(BluetoothSDPUUID16) -> Self!

Creates a new 16-bit IOBluetoothSDPUUID with the given UUID16

class func uuid32(BluetoothSDPUUID32) -> Self!

Creates a new 32-bit IOBluetoothSDPUUID with the given UUID32

## Relationships

### Inherits From

- NSData

### Conforms To

- BidirectionalCollection
- CVarArg
- Collection
- CustomDebugStringConvertible
- CustomStringConvertible
- DataProtocol
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSMutableCopying
- NSObjectProtocol
- NSSecureCoding
- RandomAccessCollection
- Sequence

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

