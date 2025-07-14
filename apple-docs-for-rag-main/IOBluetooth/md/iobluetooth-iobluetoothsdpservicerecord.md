

- IOBluetooth
-  IOBluetoothSDPServiceRecord 

Class

# IOBluetoothSDPServiceRecord

An instance of this class represents a single SDP service record.

macOS

``` source
class IOBluetoothSDPServiceRecord
```

## Overview

As a service record, an instance of this class has an NSDictionary of service attributes. It also has a link to the IOBluetoothDevice that the service belongs to. The service dictionary is keyed off of the attribute ID of each attribute represented as an NSNumber.

## Topics

### Initializers

init!(serviceDictionary: [AnyHashable : Any]!, device: IOBluetoothDevice!)

Returns an initialized IOBluetoothSDPServiceRecord \* with the attributes specified in the provided service dictionary. Provide a pointer to an IOBlueotothDevice if you wish to associate the record to a specific IOBluetoothDevice.

### Instance Properties

var attributes: [AnyHashable : Any]!

Returns an NSDictionary containing the attributes for the service.

var device: IOBluetoothDevice!

Returns the IOBluetoothDevice that the target service belongs to.

var sortedAttributes: [Any]!

Returns a sorted array of SDP attributes

### Instance Methods

func getAttributeDataElement(BluetoothSDPServiceAttributeID) -> IOBluetoothSDPDataElement!

Returns the data element for the given attribute ID in the target service.

func getHandle(UnsafeMutablePointer&lt;BluetoothSDPServiceRecordHandle>!) -> IOReturn

Allows the discovery of the service record handle assigned to the service.

func getL2CAPPSM(UnsafeMutablePointer&lt;BluetoothL2CAPPSM>!) -> IOReturn

Allows the discovery of the L2CAP PSM assigned to the service.

func getRFCOMMChannelID(UnsafeMutablePointer&lt;BluetoothRFCOMMChannelID>!) -> IOReturn

Allows the discovery of the RFCOMM channel ID assigned to the service.

func getRef() -> Unmanaged&lt;IOBluetoothSDPServiceRecordRef>!

Returns an IOBluetoothSDPServiceRecordRef representation of the target IOBluetoothSDPServiceRecord object.

func getServiceName() -> String!

Returns the name of the service.

func handsFreeSupportedFeatures() -> UInt16

func hasService(from: [Any]!) -> Bool

Returns TRUE if any one of the UUIDs in the given array is found in the target service.

func matchesSearch([Any]!) -> Bool

Returns TRUE any of the UUID arrays in the search array match the target service.

func matchesUUID16(BluetoothSDPUUID16) -> Bool

Returns TRUE the UUID16 is found in the target service.

func matchesUUIDArray([Any]!) -> Bool

Returns TRUE if ALL of the UUIDs in the given array is found in the target service.

func remove() -> IOReturn

Removes the service from the local SDP server.

### Type Methods

class func publishedServiceRecord(with: [AnyHashable : Any]!) -> Self!

Adds a service to the local SDP server.

class func withSDPServiceRecordRef(IOBluetoothSDPServiceRecordRef!) -> Self!

Method call to convert an IOBluetoothSDPServiceRecordRef into an IOBluetoothSDPServiceRecord \*.

class func withServiceDictionary([AnyHashable : Any]!, device: IOBluetoothDevice!) -> Self!

Returns an IOBluetoothSDPServiceRecord \* with the attributes specified in the provided service dictionary. Provide a pointer to an IOBlueotothDevice if you wish to associate the record to a specific IOBluetoothDevice.

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

