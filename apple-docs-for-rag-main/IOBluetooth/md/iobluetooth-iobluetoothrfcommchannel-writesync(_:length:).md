

- IOBluetooth
- IOBluetoothRFCOMMChannel
-  writeSync(\_:length:) 

Instance Method

# writeSync(\_:length:)

Sends a block of data in the channel synchronously.

macOS

``` source
func writeSync(
    _ data: UnsafeMutableRawPointer!,
    length: UInt16
) -> IOReturn
```

## Parameters 

`data`  

A pointer to the data buffer to be sent.

`length`  

The length of the buffer to be sent (in bytes).

## Return Value

Returns kIOReturnSuccess if the data was written successfully.

## Discussion

Sends data through the channel. The number of bytes to be sent must not exceed the channel MTU. If the return value is an error condition none of the data was sent. This method will block until the data has been successfully sent to the hardware for transmission (or until an error occurs).

NOTE: This method is only available in macOS 10.2.5 (Bluetooth v1.2) or later.

