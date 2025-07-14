

- IOBluetooth
-  IOBluetoothHandsFree 

Class

# IOBluetoothHandsFree

Hands free profile class.

macOS 10.7+

``` source
class IOBluetoothHandsFree
```

## Overview

Superclass of IOBluetoothHandsFreeDevice and IOBluetoothHandsFreeAudioGateway classes. Contains the common code used to support the bluetoooth hands free profile.

## Topics

### Initializers

init!(device: IOBluetoothDevice!, delegate: (any IOBluetoothHandsFreeDelegate)!)

Create a new IOBluetoothHandsFree object

### Instance Properties

var delegate: (any IOBluetoothHandsFreeDelegate)!

Return the delegate

var device: IOBluetoothDevice!

Return the IOBluetoothDevice.

var deviceCallHoldModes: UInt32

Return the device’s supported call hold modes.

var deviceSupportedFeatures: UInt32

Return the device’s supported features.

var deviceSupportedSMSServices: UInt32

Return the device’s supported SMS services.

var inputVolume: Float

Return the input volume

var isConnected: Bool

var isInputMuted: Bool

Return the input mute state.

var isOutputMuted: Bool

Return the output mute state.

var isSMSEnabled: Bool

Return YES if the device has SMS enabled.

var outputVolume: Float

Return the output volume

var smsMode: IOBluetoothSMSMode

Return the device’s SMS mode.

var supportedFeatures: UInt32

Set the supported features

### Instance Methods

func connect()

Connect to the device

func connectSCO()

Open a SCO connection with the device

func disconnect()

Disconnect from the device

func disconnectSCO()

Disconnect the SCO connection with the device

func indicator(String!) -> Int32

Return an indicator’s value

func isSCOConnected() -> Bool

Determine if there is a SCO connection to the device

func setIndicator(String!, value: Int32)

Set an indicator’s value

## Relationships

### Inherits From

- NSObject

### Inherited By

- IOBluetoothHandsFreeAudioGateway
- IOBluetoothHandsFreeDevice

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

