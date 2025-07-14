

- IOBluetooth
-  IOBluetoothRFCOMMChannelDelegate 

Protocol

# IOBluetoothRFCOMMChannelDelegate

macOS

``` source
protocol IOBluetoothRFCOMMChannelDelegate
```

## Topics

### Instance Methods

func rfcommChannelClosed(IOBluetoothRFCOMMChannel!)

func rfcommChannelControlSignalsChanged(IOBluetoothRFCOMMChannel!)

func rfcommChannelData(IOBluetoothRFCOMMChannel!, data: UnsafeMutableRawPointer!, length: Int)

func rfcommChannelFlowControlChanged(IOBluetoothRFCOMMChannel!)

func rfcommChannelOpenComplete(IOBluetoothRFCOMMChannel!, status: IOReturn)

func rfcommChannelQueueSpaceAvailable(IOBluetoothRFCOMMChannel!)

func rfcommChannelWriteComplete(IOBluetoothRFCOMMChannel!, refcon: UnsafeMutableRawPointer!, status: IOReturn)

func rfcommChannelWriteComplete(IOBluetoothRFCOMMChannel!, refcon: UnsafeMutableRawPointer!, status: IOReturn, bytesWritten: Int)

## Relationships

### Conforming Types

- IOBluetoothOBEXSession

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

protocol IOBluetoothL2CAPChannelDelegate

