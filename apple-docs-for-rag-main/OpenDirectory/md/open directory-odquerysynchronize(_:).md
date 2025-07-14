

- Open Directory
-  ODQuerySynchronize(\_:) 

Function

# ODQuerySynchronize(\_:)

Restarts a query, disposing of any results it has obtained.

Mac CatalystmacOS 10.6+

``` source
func ODQuerySynchronize(_ query: ODQueryRef!)
```

## Parameters 

`query`  

The query.

## Discussion

If `inQuery` was originally scheduled in a run loop with ODQueryScheduleWithRunLoop(_:_:_:), the query’s callback function is called with `inResults` set to `NULL`, `inError.error` set to `kODErrorQuerySynchronize`, and `inError.domain` set to `kODErrorDomainFramework`.

## See Also

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

func ODQuerySetDispatchQueue(ODQueryRef!, dispatch_queue_t!)

Retrieves results from a query asynchronously by adding the query to a dispatch queue.

func ODQueryUnscheduleFromRunLoop(ODQueryRef!, CFRunLoop!, CFString!)

Removes a query from a specified run loop.

