

- IOBluetooth
-  IOBluetoothL2CAPChannelDelegate 

Protocol

# IOBluetoothL2CAPChannelDelegate

macOS

``` source
protocol IOBluetoothL2CAPChannelDelegate
```

## Topics

### Instance Methods

func l2capChannelClosed(IOBluetoothL2CAPChannel!)

func l2capChannelData(IOBluetoothL2CAPChannel!, data: UnsafeMutableRawPointer!, length: Int)

func l2capChannelOpenComplete(IOBluetoothL2CAPChannel!, status: IOReturn)

func l2capChannelQueueSpaceAvailable(IOBluetoothL2CAPChannel!)

func l2capChannelReconfigured(IOBluetoothL2CAPChannel!)

func l2capChannelWriteComplete(IOBluetoothL2CAPChannel!, refcon: UnsafeMutableRawPointer!, status: IOReturn)

## See Also

### Protocols

protocol IOBluetoothDeviceAsyncCallbacks

protocol IOBluetoothDeviceInquiryDelegate

This category on NSObject describes the delegate methods for the IOBluetoothDeviceInquiry object. All methods are optional, but it is highly recommended you implement them all. Do NOT invoke remote name requests on found IOBluetoothDevice objects unless the inquiry object has been stopped. Doing so may deadlock your process.

protocol IOBluetoothDevicePairDelegate

protocol IOBluetoothHandsFreeAudioGatewayDelegate

A set of optional methods for receiving information about status changes for a connected Bluetooth hands-free phone or headset.

protocol IOBluetoothHandsFreeDelegate

protocol IOBluetoothHandsFreeDeviceDelegate

A set of optional methods for receiving status change updates and information about a connected Bluetooth hands-free phone or headset.

protocol IOBluetoothRFCOMMChannelDelegate

