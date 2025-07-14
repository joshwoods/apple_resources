

- IOBluetooth
-  IOBluetoothDevicePairDelegate 

Protocol

# IOBluetoothDevicePairDelegate

macOS

``` source
protocol IOBluetoothDevicePairDelegate : NSObjectProtocol
```

## Topics

### Instance Methods

func devicePairingConnected(Any!)

func devicePairingConnecting(Any!)

func devicePairingFinished(Any!, error: IOReturn)

func devicePairingPINCodeRequest(Any!)

func devicePairingStarted(Any!)

func devicePairingUserConfirmationRequest(Any!, numericValue: BluetoothNumericValue)

func devicePairingUserPasskeyNotification(Any!, passkey: BluetoothPasskey)

func deviceSimplePairingComplete(Any!, status: BluetoothHCIEventStatus)

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Protocols

protocol IOBluetoothDeviceAsyncCallbacks

protocol IOBluetoothDeviceInquiryDelegate

This category on NSObject describes the delegate methods for the IOBluetoothDeviceInquiry object. All methods are optional, but it is highly recommended you implement them all. Do NOT invoke remote name requests on found IOBluetoothDevice objects unless the inquiry object has been stopped. Doing so may deadlock your process.

protocol IOBluetoothHandsFreeAudioGatewayDelegate

A set of optional methods for receiving information about status changes for a connected Bluetooth hands-free phone or headset.

protocol IOBluetoothHandsFreeDelegate

protocol IOBluetoothHandsFreeDeviceDelegate

A set of optional methods for receiving status change updates and information about a connected Bluetooth hands-free phone or headset.

protocol IOBluetoothL2CAPChannelDelegate

protocol IOBluetoothRFCOMMChannelDelegate

