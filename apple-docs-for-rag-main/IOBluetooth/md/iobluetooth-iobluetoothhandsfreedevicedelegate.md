

- IOBluetooth
-  IOBluetoothHandsFreeDeviceDelegate 

Protocol

# IOBluetoothHandsFreeDeviceDelegate

A set of optional methods for receiving status change updates and information about a connected Bluetooth hands-free phone or headset.

macOS

``` source
protocol IOBluetoothHandsFreeDeviceDelegate : IOBluetoothHandsFreeDelegate
```

## Topics

### Receiving Status Indicator Changes

func handsFree(IOBluetoothHandsFreeDevice!, callSetupMode: NSNumber!)

Tells the delegate the call setup indicator of the connected Bluetooth hands-free phone or headset has changed.

func handsFree(IOBluetoothHandsFreeDevice!, isCallActive: NSNumber!)

Tells the delegate the active call indicator of the connected Bluetooth hands-free phone or headset has changed.

func handsFree(IOBluetoothHandsFreeDevice!, isServiceAvailable: NSNumber!)

Tells the delegate the service level indicator of the connected Bluetooth hands-free phone or headset has changed.

func handsFree(IOBluetoothHandsFreeDevice!, signalStrength: NSNumber!)

Tells the delegate the call setup signal strength indicator of the connected Bluetooth hands-free phone or headset has changed.

func handsFree(IOBluetoothHandsFreeDevice!, callHoldState: NSNumber!)

Tells the delegate the call held indicator of the connected Bluetooth hands-free phone or headset has changed.

func handsFree(IOBluetoothHandsFreeDevice!, isRoaming: NSNumber!)

Tells the delegate the roaming indicator of the connected Bluetooth hands-free phone or headset has changed.

func handsFree(IOBluetoothHandsFreeDevice!, batteryCharge: NSNumber!)

Tells the delegate the battery level indicator of the connected Bluetooth hands-free phone or headset has changed.

### Receiving Call Status

func handsFree(IOBluetoothHandsFreeDevice!, incomingCallFrom: String!)

Tells the delegate there’s an incoming call on the connected Bluetooth hands-free phone or headset.

func handsFree(IOBluetoothHandsFreeDevice!, currentCall: [AnyHashable : Any]!)

Sends the delegate information about the current call.

Current Call Information Constants

Get information about a phone call on a hands-free Bluetooth device.

### Receiving SMS Information

func handsFree(IOBluetoothHandsFreeDevice!, incomingSMS: [AnyHashable : Any]!)

Tells the delegate there’s an incoming text message.

SMS Dictionary Key Constants

Read the parts of an SMS message.

### Receiving Other Information

func handsFree(IOBluetoothHandsFreeDevice!, subscriberNumber: String!)

Tells the delegate the subscriber number of a call.

func handsFree(IOBluetoothHandsFreeDevice!, ringAttempt: NSNumber!)

Tells the delegate the phone is ringing.

func handsFree(IOBluetoothHandsFreeDevice!, unhandledResultCode: String!)

Tells the delegate the phone sent an unknown code.

## Relationships

### Inherits From

- IOBluetoothHandsFreeDelegate
- NSObjectProtocol

## See Also

### Protocols

protocol IOBluetoothDeviceAsyncCallbacks

protocol IOBluetoothDeviceInquiryDelegate

This category on NSObject describes the delegate methods for the IOBluetoothDeviceInquiry object. All methods are optional, but it is highly recommended you implement them all. Do NOT invoke remote name requests on found IOBluetoothDevice objects unless the inquiry object has been stopped. Doing so may deadlock your process.

protocol IOBluetoothDevicePairDelegate

protocol IOBluetoothHandsFreeAudioGatewayDelegate

A set of optional methods for receiving information about status changes for a connected Bluetooth hands-free phone or headset.

protocol IOBluetoothHandsFreeDelegate

protocol IOBluetoothL2CAPChannelDelegate

protocol IOBluetoothRFCOMMChannelDelegate

