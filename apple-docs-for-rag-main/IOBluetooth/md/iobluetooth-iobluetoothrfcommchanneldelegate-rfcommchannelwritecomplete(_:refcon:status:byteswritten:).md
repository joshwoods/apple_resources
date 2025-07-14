

- IOBluetooth
- IOBluetoothRFCOMMChannelDelegate
-  rfcommChannelWriteComplete(\_:refcon:status:bytesWritten:) 

Instance Method

# rfcommChannelWriteComplete(\_:refcon:status:bytesWritten:)

macOS

``` source
optional func rfcommChannelWriteComplete(
    _ rfcommChannel: IOBluetoothRFCOMMChannel!,
    refcon: UnsafeMutableRawPointer!,
    status error: IOReturn,
    bytesWritten length: Int
)
```

