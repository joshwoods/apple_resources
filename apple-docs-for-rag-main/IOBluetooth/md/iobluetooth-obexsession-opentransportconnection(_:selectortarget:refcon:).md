

- IOBluetooth
- OBEXSession
-  openTransportConnection(\_:selectorTarget:refCon:) 

Instance Method

# openTransportConnection(\_:selectorTarget:refCon:)

Opens a transport connection to a device. A Bluetooth connection is one example of a transport.

macOS

``` source
func openTransportConnection(
    _ inSelector: Selector!,
    selectorTarget inTarget: Any!,
    refCon inUserRefCon: UnsafeMutableRawPointer!
) -> OBEXError
```

## Parameters 

`inSelector`  

Selector to call for success, failure or timeout.

`inTarget`  

Target on which to call the selector.

`inUserRefCon`  

Caller’s reference constant.

## Discussion

Tranport subclasses must override this! when called you should attempt to open your transport connection, and if you are successful, return kOBEXSuccess, otherwise an interesting error code.

