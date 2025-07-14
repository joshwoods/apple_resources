

- Core Services
- File Metadata
- MDQuery
-  MDQuerySetSearchScope(\_:\_:\_:) 

Function

# MDQuerySetSearchScope(\_:\_:\_:)

Sets the search scope for a query instance.

macOS 10.4+

``` source
func MDQuerySetSearchScope(
    _ query: MDQuery!,
    _ scopeDirectories: CFArray!,
    _ scopeOptions: OptionBits
)
```

## Parameters 

`query`  

The query object to modify.

`scopeDirectories`  

A CFArray of CFStringRef or CFURLRef objects which specify where to search. For convenience the `kMDQueryScopeHome`, `kMDQueryScopeComputer` and `kMDQueryScopeNetwork` constants may also be included in the array.

`scopeOptions`  

Additional options for modifying the search. Currently you must pass 0.

## Discussion

## See Also

### Creating Queries

func MDQueryCreate(CFAllocator!, CFString!, CFArray!, CFArray!) -> MDQuery!

Creates a new query instance.

func MDQueryCreateSubset(CFAllocator!, MDQuery!, CFString!, CFArray!, CFArray!) -> MDQuery!

Creates a new query that is a subset of the specified parentquery.

func MDQuerySetDispatchQueue(MDQuery!, dispatch_queue_t!)

Sets the dispatch queue on which query results will be delivered by MDQueryExecute.

