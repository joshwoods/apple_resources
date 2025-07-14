

- IOBluetooth
- IOBluetoothL2CAPChannel
-  writeSync(\_:length:) 

Instance Method

# writeSync(\_:length:)

Writes the given data synchronously over the target L2CAP channel to the remote device.

macOS

``` source
func writeSync(
    _ data: UnsafeMutableRawPointer!,
    length: UInt16
) -> IOReturn
```

## Parameters 

`data`  

Pointer to the buffer containing the data to send.

`length`  

The length of the given data buffer.

## Return Value

Returns kIOReturnSuccess if the data was written successfully.

## Discussion

The length of the data may not exceed the L2CAP channel’s ougoing MTU. This method will block until the data has been successfully sent to the hardware for transmission (or an error occurs).

NOTE: This method is only available in macOS 10.2.5 (Bluetooth v1.2) or later.

