

- Core Services
- File Metadata
- MDQuery
-  MDQueryCopyValueListAttributes(\_:) 

Function

# MDQueryCopyValueListAttributes(\_:)

Returns the list of attribute names for which values are being collected by the query.

macOS 10.4+

``` source
func MDQueryCopyValueListAttributes(_ query: MDQuery!) -> CFArray!
```

## Parameters 

`query`  

The query.

## Return Value

A CFArrayRef containing the attribute names of the collected values.

## See Also

### Getting and Setting Query Parameters

func MDQuerySetMaxCount(MDQuery!, CFIndex)

Sets the maximum number of results returned.

func MDQueryGetBatchingParameters(MDQuery!) -> MDQueryBatchingParams

Returns the current parameters that control the batching of progress notifications.

func MDQuerySetBatchingParameters(MDQuery!, MDQueryBatchingParams)

Set the query batching parameters.

func MDQueryCopySortingAttributes(MDQuery!) -> CFArray!

Returns the list of attribute names used to sort the results.

func MDQueryCopyQueryString(MDQuery!) -> CFString!

Returns the query string of the query.

