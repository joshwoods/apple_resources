

- Open Directory
-  ODQuerySetDispatchQueue(\_:\_:) 

Function

# ODQuerySetDispatchQueue(\_:\_:)

Retrieves results from a query asynchronously by adding the query to a dispatch queue.

Mac CatalystmacOS 10.6+

``` source
func ODQuerySetDispatchQueue(
    _ query: ODQueryRef!,
    _ queue: dispatch_queue_t!
)
```

## Parameters 

`query`  

The query.

`queue`  

The dispatch queue.

## Discussion

When the query is complete, the query’s callback function is called with both `inResults` and `inError` set to `NULL`.

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

func ODQueryScheduleWithRunLoop(ODQueryRef!, CFRunLoop!, CFString!)

Retrieves results from a query asynchronously by scheduling the query in a run loop.

func ODQuerySetCallback(ODQueryRef!, ODQueryCallback!, UnsafeMutableRawPointer!)

Sets the callback for an asynchronous query.

func ODQuerySynchronize(ODQueryRef!)

Restarts a query, disposing of any results it has obtained.

func ODQueryUnscheduleFromRunLoop(ODQueryRef!, CFRunLoop!, CFString!)

Removes a query from a specified run loop.

