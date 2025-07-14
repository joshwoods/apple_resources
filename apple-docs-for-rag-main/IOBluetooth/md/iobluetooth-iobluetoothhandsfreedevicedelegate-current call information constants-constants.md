

- IOBluetooth
- IOBluetoothHandsFreeDeviceDelegate
-  Current Call Information Constants 

API Collection

# Current Call Information Constants

Get information about a phone call on a hands-free Bluetooth device.

## Topics

### Call Information

let IOBluetoothHandsFreeCallDirection: String

A value that indicates whether a call is incoming or outgoing.

let IOBluetoothHandsFreeCallIndex: String

The index of the call, starting with `1`.

let IOBluetoothHandsFreeCallMode: String

The type of call data.

let IOBluetoothHandsFreeCallMultiparty: String

A value that indicates whether the call is multiple-party.

let IOBluetoothHandsFreeCallStatus: String

The current state of the call.

### Remote Number Information

let IOBluetoothHandsFreeCallNumber: String

The caller’s phone number.

let IOBluetoothHandsFreeCallType: String

The format of the caller’s phone number.

let IOBluetoothHandsFreeCallName: String

The name of the caller.

## See Also

### Receiving Call Status

func handsFree(IOBluetoothHandsFreeDevice!, incomingCallFrom: String!)

Tells the delegate there’s an incoming call on the connected Bluetooth hands-free phone or headset.

func handsFree(IOBluetoothHandsFreeDevice!, currentCall: [AnyHashable : Any]!)

Sends the delegate information about the current call.

