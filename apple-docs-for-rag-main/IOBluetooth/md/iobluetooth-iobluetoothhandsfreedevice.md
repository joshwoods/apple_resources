

- IOBluetooth
-  IOBluetoothHandsFreeDevice 

Class

# IOBluetoothHandsFreeDevice

An object you use to manage phone calls on a connected Bluetooth hands-free phone or headset.

macOS 10.7+

``` source
class IOBluetoothHandsFreeDevice
```

## Topics

### Creating a Hands-Free Device Manager

init!(device: IOBluetoothDevice!, delegate: Any!)

Creates an object to manage phone calls on a hands-free Bluetooth device.

### Accepting Calls

func acceptCall()

Accepts an incoming call.

func acceptCallOnPhone()

Accepts an incoming call and transfers the audio to the managed hands-free phone or headset.

func callTransfer()

Ends all calls that are active or on hold, and accepts any waiting calls.

### Dialing Calls

func dialNumber(String!)

Calls the phone number on a hands-free phone or headset.

func memoryDial(Int32)

Calls the phone number stored in a speed dial or memory slot of the hands-free phone or headset.

func redial()

Calls the number stored on the hands-free phone or headset again.

### Holding Calls

func holdCall()

Places all active calls on hold and accepts a held or waiting call.

func addHeldCall()

Adds held calls to the current conversation.

func placeAllOthers(onHold: Int32)

Places all calls except the call with the specified index on hold.

### Ending Calls

func endCall()

Ends the current call or refuses an incoming call.

func releaseCall(Int32)

Ends the call with the specified index.

func releaseActiveCalls()

Ends all active calls and accepts a held or waiting call.

func releaseHeldCalls()

Ends all calls that are on hold or returns a busy signal for a waiting call.

### Sending Messages and Commands

func sendSMS(String!, message: String!)

Sends a text message to a phone number.

func sendDTMF(String!)

Sends the tone associated with a phone key to the hands-free Bluetooth device.

func send(atCommand: String!)

Sends an AT command to the Bluetooth audio gateway.

func send(atCommand: String!, timeout: Float, selector: Selector!, target: Any!)

Send an AT command to the Bluetooth audio gateway and performs a selector on completion or timeout.

### Requesting Status Information

func subscriberNumber()

Requests that the Bluetooth audio gateway send the subscriber number to the delegate.

func currentCallList()

Requests that the Bluetooth audio gateway send the delegate a list of calls that are active, on hold, or being set up.

### Transferring Audio

func transferAudioToComputer()

Moves the audio for current and future calls to a Mac.

func transferAudioToPhone()

Moves the audio for current or future calls to a phone.

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

class IOBluetoothHandsFreeAudioGateway

An object that sends data to a connected Bluetooth hands-free phone or headset and processes commands from it.

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

