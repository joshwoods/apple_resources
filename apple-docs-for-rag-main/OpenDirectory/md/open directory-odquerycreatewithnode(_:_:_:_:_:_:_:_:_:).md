

- Open Directory
-  ODQueryCreateWithNode(\_:\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# ODQueryCreateWithNode(\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Creates a query with a node using provided parameters.

Mac CatalystmacOS 10.6+

``` source
func ODQueryCreateWithNode(
    _ allocator: CFAllocator!,
    _ node: ODNodeRef!,
    _ recordTypeOrList: CFTypeRef!,
    _ attribute: String!,
    _ matchType: ODMatchType,
    _ queryValueOrList: CFTypeRef!,
    _ returnAttributeOrList: CFTypeRef!,
    _ maxResults: CFIndex,
    _ error: UnsafeMutablePointer?>!
) -> Unmanaged!
```

## Parameters 

`allocator`  

The memory allocator to use. If `NULL`, the default allocator is used.

`node`  

The node.

`recordTypeOrList`  

The type or types of record to query. Can be a `CFString` object for a single type or a `CFArray` object containing `CFString` objects for multiple types.

`attribute`  

The name of the attribute to query.

`matchType`  

The type of query.

`queryValueOrList`  

The value or values to query in the attribute. Can be a `CFString` object or a `CFData` object for a single value, or a `CFArray` containing `CFString` and `CFData` objects for multiple values.

`returnAttributeOrList`  

The attribute or attributes to be returned from the query. Can be a `CFString` object for a single attribute or a `CFArray` object containing `CFString` objects for multiple attributes. Passing `NULL` is equivalent to passing `kODAttributeTypeStandardOnly`.

`maxResults`  

The maximum number of values to be returned.

`error`  

An error reference for error details. Can be `NULL`.

## Return Value

The created query.

## See Also

### Working with Queries

func ODQueryCopyResults(ODQueryRef!, Bool, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFArray>!

Returns results from a query synchronously.

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

