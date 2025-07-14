

- Core Foundation
-  CFSocketCallBack 

Type Alias

# CFSocketCallBack

Callback invoked when certain types of activity takes place on a CFSocket object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFSocketCallBack = (CFSocket?, CFSocketCallBackType, CFData?, UnsafeRawPointer?, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`s`  

The CFSocket object that experienced some activity.

`callbackType`  

The type of activity detected.

`address`  

A CFData object holding the contents of a `struct sockaddr` appropriate for the protocol family of `s` (`struct sockaddr_in` or `struct sockaddr_in6`, for example), identifying the remote address to which `s` is connected. This value is `NULL` except for `kCFSocketAcceptCallBack` and `kCFSocketDataCallBack` callbacks.

`data`  

Data appropriate for the callback type. For a `kCFSocketConnectCallBack` that failed in the background, it is a pointer to an `SInt32` error code; for a `kCFSocketAcceptCallBack`, it is a pointer to a CFSocketNativeHandle; or for a `kCFSocketDataCallBack`, it is a CFData object containing the incoming data. In all other cases, it is `NULL`.

`info`  

The `info` member of the CFSocketContext structure that was used when creating the CFSocket object.

## Discussion

You specify this callback when you create the CFSocket object with CFSocketCreate(_:_:_:_:_:_:_:), CFSocketCreateConnectedToSocketSignature(_:_:_:_:_:_:), CFSocketCreateWithNative(_:_:_:_:_:), or CFSocketCreateWithSocketSignature(_:_:_:_:_:).

