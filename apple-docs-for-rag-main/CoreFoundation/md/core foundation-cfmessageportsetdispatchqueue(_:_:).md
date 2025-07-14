

- Core Foundation
-  CFMessagePortSetDispatchQueue(\_:\_:) 

Function

# CFMessagePortSetDispatchQueue(\_:\_:)

Schedules callbacks for the specified message port on the specified dispatch queue.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFMessagePortSetDispatchQueue(
    _ ms: CFMessagePort!,
    _ queue: dispatch_queue_t!
)
```

## Parameters 

`ms`  

The message port to schedule.

`queue`  

The libdispatch queue.

## See Also

### Using a Message Port

func CFMessagePortInvalidate(CFMessagePort!)

Invalidates a CFMessagePort object, stopping it from receiving or sending any more messages.

func CFMessagePortSendRequest(CFMessagePort!, Int32, CFData!, CFTimeInterval, CFTimeInterval, CFString!, UnsafeMutablePointer&lt;Unmanaged&lt;CFData>?>!) -> Int32

Sends a message to a remote CFMessagePort object.

