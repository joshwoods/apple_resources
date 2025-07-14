

- IOBluetooth
-  IOBluetoothHandsFreeAudioGateway 

Class

# IOBluetoothHandsFreeAudioGateway

An object that sends data to a connected Bluetooth hands-free phone or headset and processes commands from it.

macOS 10.7+

``` source
class IOBluetoothHandsFreeAudioGateway
```

## Overview

This class represents the audio gateway portion of a Bluetooth audio profile.

## Topics

### Creating a Gateway

init!(device: IOBluetoothDevice!, delegate: Any!)

Creates an object that controls a connected Bluetooth hands-free phone or headset.

### Showing Status Indicators

func createIndicator(String!, min: Int32, max: Int32, currentValue: Int32)

Sends a request to the Bluetooth device to show or update a status indicator.

Status Indicator Constants

Send commands to modify the status indicators of a hands-free Bluetooth device.

### Sending and Receiving Commands

func sendResponse(String!)

Sends data followed by a success message to a connected Bluetooth hands-free phone or headset.

func sendResponse(String!, withOK: Bool)

Sends data followed by an optional success message to a connected Bluetooth hands-free phone or headset.

func sendOKResponse()

Sends a success message to a connected Bluetooth hands-free phone or headset.

func process(atCommand: String!)

Processes a command from a connected Bluetooth hands-free phone or headset.

## Relationships

### Inherits From

- IOBluetoothHandsFree

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

class IOBluetoothDeviceInquiry

Object representing a device inquiry that finds Bluetooth devices in-range of the computer, and (optionally) retrieves name information for them.

class IOBluetoothDevicePair

An instance of IOBluetoothDevicePair represents a pairing attempt to a remote Bluetooth device.

class IOBluetoothDeviceRef

An object that represents a Bluetooth I/O device.

class IOBluetoothHandsFree

Hands free profile class.

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

