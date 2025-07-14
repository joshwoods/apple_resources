

- Core Foundation
-  CFMessagePortCallBack 

Type Alias

# CFMessagePortCallBack

Callback invoked to process a message received on a CFMessagePort object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFMessagePortCallBack = (CFMessagePort?, Int32, CFData?, UnsafeMutableRawPointer?) -> Unmanaged?
```

## Parameters 

`local`  

The local message port that received the message.

`msgid`  

An arbitrary integer value assigned to the message by the sender.

`data`  

The message data.

`info`  

The `info` member of the CFMessagePortContext structure that was used when creating `local`.

## Return Value

Data to send back to the sender of the message. The system releases the returned CFData object. Return `NULL` if you want an empty reply returned to the sender.

## Discussion

If you want the message data to persist beyond this callback, you must explicitly create a copy of `data` rather than merely retain it; the contents of `data` will be deallocated after the callback exits.

## See Also

### Callbacks

typealias CFMessagePortInvalidationCallBack

Callback invoked when a CFMessagePort object is invalidated.

