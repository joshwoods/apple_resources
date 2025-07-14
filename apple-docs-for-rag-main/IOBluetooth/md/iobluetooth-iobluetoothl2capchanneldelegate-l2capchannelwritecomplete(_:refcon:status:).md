

- IOBluetooth
- IOBluetoothL2CAPChannelDelegate
-  l2capChannelWriteComplete(\_:refcon:status:) 

Instance Method

# l2capChannelWriteComplete(\_:refcon:status:)

macOS

``` source
optional func l2capChannelWriteComplete(
    _ l2capChannel: IOBluetoothL2CAPChannel!,
    refcon: UnsafeMutableRawPointer!,
    status error: IOReturn
)
```

