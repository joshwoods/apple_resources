

- IOBluetooth
-  IOBluetoothDeviceInquiryDelegate 

Protocol

# IOBluetoothDeviceInquiryDelegate

This category on NSObject describes the delegate methods for the IOBluetoothDeviceInquiry object. All methods are optional, but it is highly recommended you implement them all. Do NOT invoke remote name requests on found IOBluetoothDevice objects unless the inquiry object has been stopped. Doing so may deadlock your process.

macOS

``` source
protocol IOBluetoothDeviceInquiryDelegate : NSObjectProtocol
```

## Topics

### Instance Methods

func deviceInquiryComplete(IOBluetoothDeviceInquiry!, error: IOReturn, aborted: Bool)

func deviceInquiryDeviceFound(IOBluetoothDeviceInquiry!, device: IOBluetoothDevice!)

func deviceInquiryDeviceNameUpdated(IOBluetoothDeviceInquiry!, device: IOBluetoothDevice!, devicesRemaining: UInt32)

func deviceInquiryStarted(IOBluetoothDeviceInquiry!)

func deviceInquiryUpdatingDeviceNamesStarted(IOBluetoothDeviceInquiry!, devicesRemaining: UInt32)

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Protocols

protocol IOBluetoothDeviceAsyncCallbacks

protocol IOBluetoothDevicePairDelegate

protocol IOBluetoothHandsFreeAudioGatewayDelegate

A set of optional methods for receiving information about status changes for a connected Bluetooth hands-free phone or headset.

protocol IOBluetoothHandsFreeDelegate

protocol IOBluetoothHandsFreeDeviceDelegate

A set of optional methods for receiving status change updates and information about a connected Bluetooth hands-free phone or headset.

protocol IOBluetoothL2CAPChannelDelegate

protocol IOBluetoothRFCOMMChannelDelegate

