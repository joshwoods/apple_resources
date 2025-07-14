

- Open Directory
-  ODQueryCopyResults(\_:\_:\_:) 

Function

# ODQueryCopyResults(\_:\_:\_:)

Returns results from a query synchronously.

Mac CatalystmacOS 10.6+

``` source
func ODQueryCopyResults(
    _ query: ODQueryRef!,
    _ allowPartialResults: Bool,
    _ error: UnsafeMutablePointer?>!
) -> Unmanaged!
```

## Parameters 

`query`  

The query.

`allowPartialResults`  

If `true`, only immediately available results are returned; otherwise, the function waits until all results are available.

`error`  

An error reference for error details. Can be `NULL`.

## Return Value

The results of the query in an array of `ODRecord` objects.

## See Also

### Working with Queries

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

func ODQuerySetDispatchQueue(ODQueryRef!, dispatch_queue_t!)

Retrieves results from a query asynchronously by adding the query to a dispatch queue.

func ODQuerySynchronize(ODQueryRef!)

Restarts a query, disposing of any results it has obtained.

func ODQueryUnscheduleFromRunLoop(ODQueryRef!, CFRunLoop!, CFString!)

Removes a query from a specified run loop.

