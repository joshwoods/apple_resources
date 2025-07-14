

- IOBluetooth
-  IOBluetoothHandsFreeDelegate 

Protocol

# IOBluetoothHandsFreeDelegate

macOS

``` source
protocol IOBluetoothHandsFreeDelegate : NSObjectProtocol
```

## Topics

### Instance Methods

func handsFree(IOBluetoothHandsFree!, connected: NSNumber!)

func handsFree(IOBluetoothHandsFree!, disconnected: NSNumber!)

func handsFree(IOBluetoothHandsFree!, scoConnectionClosed: NSNumber!)

func handsFree(IOBluetoothHandsFree!, scoConnectionOpened: NSNumber!)

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- IOBluetoothHandsFreeDeviceDelegate

## See Also

### Protocols

protocol IOBluetoothDeviceAsyncCallbacks

protocol IOBluetoothDeviceInquiryDelegate

This category on NSObject describes the delegate methods for the IOBluetoothDeviceInquiry object. All methods are optional, but it is highly recommended you implement them all. Do NOT invoke remote name requests on found IOBluetoothDevice objects unless the inquiry object has been stopped. Doing so may deadlock your process.

protocol IOBluetoothDevicePairDelegate

protocol IOBluetoothHandsFreeAudioGatewayDelegate

A set of optional methods for receiving information about status changes for a connected Bluetooth hands-free phone or headset.

protocol IOBluetoothHandsFreeDeviceDelegate

A set of optional methods for receiving status change updates and information about a connected Bluetooth hands-free phone or headset.

protocol IOBluetoothL2CAPChannelDelegate

protocol IOBluetoothRFCOMMChannelDelegate

