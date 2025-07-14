

- Core Foundation
-  CFMessagePortInvalidate(\_:) 

Function

# CFMessagePortInvalidate(\_:)

Invalidates a CFMessagePort object, stopping it from receiving or sending any more messages.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFMessagePortInvalidate(_ ms: CFMessagePort!)
```

## Parameters 

`ms`  

The message port to invalidate.

## Discussion

Invalidating a message port prevents the port from ever sending or receiving any more messages; the message port is not deallocated, though. If the port has not already been invalidated, the port’s invalidation callback function is invoked, if one has been set with CFMessagePortSetInvalidationCallBack(_:_:). The CFMessagePortContext `info` information for `ms` is also released, if a release callback was specified in the port’s context structure. Finally, if a run loop source was created for `ms`, the run loop source is also invalidated.

## See Also

### Using a Message Port

func CFMessagePortSendRequest(CFMessagePort!, Int32, CFData!, CFTimeInterval, CFTimeInterval, CFString!, UnsafeMutablePointer&lt;Unmanaged&lt;CFData>?>!) -> Int32

Sends a message to a remote CFMessagePort object.

func CFMessagePortSetDispatchQueue(CFMessagePort!, dispatch_queue_t!)

Schedules callbacks for the specified message port on the specified dispatch queue.

