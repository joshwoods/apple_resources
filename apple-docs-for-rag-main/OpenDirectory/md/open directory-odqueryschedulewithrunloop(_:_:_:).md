

- Open Directory
-  ODQueryScheduleWithRunLoop(\_:\_:\_:) 

Function

# ODQueryScheduleWithRunLoop(\_:\_:\_:)

Retrieves results from a query asynchronously by scheduling the query in a run loop.

Mac CatalystmacOS 10.6+

``` source
func ODQueryScheduleWithRunLoop(
    _ query: ODQueryRef!,
    _ runLoop: CFRunLoop!,
    _ runLoopMode: CFString!
)
```

## Parameters 

`query`  

The query.

`runLoop`  

The run loop.

`runLoopMode`  

The mode of the run loop.

## Discussion

This function spawns a new thread to execute the query in `inRunLoop`. When the query is complete, the query’s callback function is called with both `inResults` and `inError` set to `NULL`. To remove an incomplete query from its run loop, call ODQueryUnscheduleFromRunLoop(_:_:_:).

## See Also

### Related Documentation

typealias ODQueryCallback

A callback function called as results from a scheduled query are returned.

### Working with Queries

func ODQueryCopyResults(ODQueryRef!, Bool, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFArray>!

Returns results from a query synchronously.

func ODQueryCreateWithNode(CFAllocator!, ODNodeRef!, CFTypeRef!, String!, ODMatchType, CFTypeRef!, CFTypeRef!, CFIndex, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;ODQueryRef>!

Creates a query with a node using provided parameters.

func ODQueryCreateWithNodeType(CFAllocator!, ODNodeType, CFTypeRef!, String!, ODMatchType, CFTypeRef!, CFTypeRef!, CFIndex, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;ODQueryRef>!

Creates a query for a particular node type using provided parameters.

func ODQueryGetTypeID() -> CFTypeID

Returns the type ID for an Open Directory query.

func ODQuerySetCallback(ODQueryRef!, ODQueryCallback!, UnsafeMutableRawPointer!)

Sets the callback for an asynchronous query.

func ODQuerySetDispatchQueue(ODQueryRef!, dispatch_queue_t!)

Retrieves results from a query asynchronously by adding the query to a dispatch queue.

func ODQuerySynchronize(ODQueryRef!)

Restarts a query, disposing of any results it has obtained.

func ODQueryUnscheduleFromRunLoop(ODQueryRef!, CFRunLoop!, CFString!)

Removes a query from a specified run loop.

