

- Core Services
- File Metadata
- MDQuery
-  MDQueryCopySortingAttributes(\_:) 

Function

# MDQueryCopySortingAttributes(\_:)

Returns the list of attribute names used to sort the results.

macOS 10.4+

``` source
func MDQueryCopySortingAttributes(_ query: MDQuery!) -> CFArray!
```

## Parameters 

`query`  

The query.

## Return Value

A CFArrayRef containing the attribute names used to sort the query results.

## See Also

### Getting and Setting Query Parameters

func MDQuerySetMaxCount(MDQuery!, CFIndex)

Sets the maximum number of results returned.

func MDQueryGetBatchingParameters(MDQuery!) -> MDQueryBatchingParams

Returns the current parameters that control the batching of progress notifications.

func MDQuerySetBatchingParameters(MDQuery!, MDQueryBatchingParams)

Set the query batching parameters.

func MDQueryCopyValueListAttributes(MDQuery!) -> CFArray!

Returns the list of attribute names for which values are being collected by the query.

func MDQueryCopyQueryString(MDQuery!) -> CFString!

Returns the query string of the query.

