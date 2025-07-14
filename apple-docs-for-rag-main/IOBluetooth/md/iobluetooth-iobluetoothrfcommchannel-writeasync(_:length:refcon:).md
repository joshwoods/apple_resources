

- IOBluetooth
- IOBluetoothRFCOMMChannel
-  writeAsync(\_:length:refcon:) 

Instance Method

# writeAsync(\_:length:refcon:)

Sends a block of data in the channel asynchronously.

macOS

``` source
func writeAsync(
    _ data: UnsafeMutableRawPointer!,
    length: UInt16,
    refcon: UnsafeMutableRawPointer!
) -> IOReturn
```

## Parameters 

`data`  

A pointer to the data buffer to be sent.

`length`  

The length of the buffer to be sent (in bytes).

`refcon`  

User supplied value that gets passed to the write callback.

## Return Value

Returns kIOReturnSuccess if the data was buffered successfully.

## Discussion

The number of bytes to be sent must not exceed the channel MTU. If the return value is an error condition none of the data was sent. Once the data has been successfully passed to the hardware to be transmitted, the delegate method -rfcommChannelWriteComplete:refcon:status: will be called with the refcon that was passed to this method.

NOTE: This method is only available in macOS 10.2.5 (Bluetooth v1.2) or later.

