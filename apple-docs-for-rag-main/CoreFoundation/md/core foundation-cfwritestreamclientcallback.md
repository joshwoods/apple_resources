

- Core Foundation
-  CFWriteStreamClientCallBack 

Type Alias

# CFWriteStreamClientCallBack

Callback invoked when certain types of activity takes place on a writable stream.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFWriteStreamClientCallBack = (CFWriteStream?, CFStreamEventType, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`stream`  

The stream that experienced the event `eventType`.

`eventType`  

The event that caused the callback to be called. The possible events are listed in CFStreamEventType.

`clientCallBackInfo`  

The `info` member of the CFStreamClientContext structure that was used when setting the client for `stream`.

## Discussion

This callback is called only for the events requested when setting the client with CFWriteStreamSetClient(_:_:_:_:).

