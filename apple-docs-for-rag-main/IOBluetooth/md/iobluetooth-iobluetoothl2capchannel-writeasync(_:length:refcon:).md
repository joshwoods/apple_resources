

- IOBluetooth
- IOBluetoothL2CAPChannel
-  writeAsync(\_:length:refcon:) 

Instance Method

# writeAsync(\_:length:refcon:)

Writes the given data over the target L2CAP channel asynchronously to the remote device.

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

Pointer to the buffer containing the data to send.

`length`  

The length of the given data buffer.

`refcon`  

User supplied value that gets passed to the write callback.

## Return Value

Returns kIOReturnSuccess if the data was buffered successfully.

## Discussion

The length of the data may not exceed the L2CAP channel’s ougoing MTU. When the data has been successfully passed to the hardware to be transmitted, the delegate method -l2capChannelWriteComplete:refcon:status: will be called with the refcon passed into this method.

NOTE: This method is only available in macOS 10.2.5 (Bluetooth v1.2) or later.

