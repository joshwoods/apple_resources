

- IOBluetooth
- IOBluetoothRFCOMMChannelDelegate
-  rfcommChannelWriteComplete(\_:refcon:status:) 

Instance Method

# rfcommChannelWriteComplete(\_:refcon:status:)

macOS

``` source
optional func rfcommChannelWriteComplete(
    _ rfcommChannel: IOBluetoothRFCOMMChannel!,
    refcon: UnsafeMutableRawPointer!,
    status error: IOReturn
)
```

