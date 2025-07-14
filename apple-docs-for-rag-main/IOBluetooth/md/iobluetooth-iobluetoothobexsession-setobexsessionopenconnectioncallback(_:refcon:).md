

- IOBluetooth
- IOBluetoothOBEXSession
-  setOBEXSessionOpenConnectionCallback(\_:refCon:) 

Instance Method

# setOBEXSessionOpenConnectionCallback(\_:refCon:)

For C API support. Allows you to set the callback to be invoked when the OBEX connection is actually opened.

macOS

``` source
func setOBEXSessionOpenConnectionCallback(
    _ inCallback: IOBluetoothOBEXSessionOpenConnectionCallback!,
    refCon inUserRefCon: UnsafeMutableRawPointer!
)
```

## Parameters 

`inCallback`  

Function to call on the target.

`inUserRefCon`  

User’s reference constant, will be returned on the callback.

