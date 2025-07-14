

- IOBluetooth
-  IOBluetoothDeviceInquiry 

Class

# IOBluetoothDeviceInquiry

Object representing a device inquiry that finds Bluetooth devices in-range of the computer, and (optionally) retrieves name information for them.

macOS

``` source
class IOBluetoothDeviceInquiry
```

## Overview

You should only use this object if your application needs to know about in-range devices and cannot use the GUI provided by the IOBluetoothUI framework. It will not let you perform unlimited back-to-back inquiries, but will instead throttle the number of attempted inquiries if too many are attempted within a small window of time. Important Note: DO NOT perform remote name requests on devices from delegate methods or while this object is in use. If you wish to do your own remote name requests on devices, do them after you have stopped this object. If you do not heed this warning, you could potentially deadlock your process.

## Topics

### Initializers

init!(delegate: Any!)

Initializes an alloc’d inquiry object, and sets the delegate object, as if -setDelegate: were called on it.

### Instance Properties

var delegate: AnyObject?

var inquiryLength: UInt8

Set the length of the inquiry that is performed each time -start is used on an inquiry object.

var searchType: IOBluetoothDeviceSearchTypes

Set the devices that are found.

var updateNewDeviceNames: Bool

Sets whether or not the inquiry object will retrieve the names of devices found during the search.

### Instance Methods

func clearFoundDevices()

Removes all found devices from the inquiry object.

func foundDevices() -> [Any]!

Returns found IOBluetoothDevice objects as an array.

func setSearchCriteria(BluetoothServiceClassMajor, majorDeviceClass: BluetoothDeviceClassMajor, minorDeviceClass: BluetoothDeviceClassMinor)

Use this method to set the criteria for the device search.

func start() -> IOReturn

Tells inquiry object to begin the inquiry and name updating process, if specified.

func stop() -> IOReturn

Halts the inquiry object. Could either stop the search for new devices, or the updating of found device names.

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

### Classes

class IOBluetoothDevice

An instance of IOBluetoothDevice represents a single remote Bluetooth device.

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

class IOBluetoothSDPDataElement

An instance of this class represents a single SDP data element as defined by the Bluetooth SDP spec.

