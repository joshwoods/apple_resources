

- Core Services
- File Metadata
- MDQuery
-  MDQuerySetDispatchQueue(\_:\_:) 

Function

# MDQuerySetDispatchQueue(\_:\_:)

Sets the dispatch queue on which query results will be delivered by MDQueryExecute.

macOS 10.6+

``` source
func MDQuerySetDispatchQueue(
    _ query: MDQuery!,
    _ queue: dispatch_queue_t!
)
```

## Parameters 

`query`  

The query.

`queue`  

The dispatch queue on which results should be delivered.

## Discussion

It is not advisable to change set dispatch queue after MDQueryExecute(_:_:) has been called with the query.

Setting the dispatch queue for a synchronous query (kMDQuerySynchronous) has no effect.

## See Also

### Creating Queries

func MDQueryCreate(CFAllocator!, CFString!, CFArray!, CFArray!) -> MDQuery!

Creates a new query instance.

func MDQueryCreateSubset(CFAllocator!, MDQuery!, CFString!, CFArray!, CFArray!) -> MDQuery!

Creates a new query that is a subset of the specified parentquery.

func MDQuerySetSearchScope(MDQuery!, CFArray!, OptionBits)

Sets the search scope for a query instance.

