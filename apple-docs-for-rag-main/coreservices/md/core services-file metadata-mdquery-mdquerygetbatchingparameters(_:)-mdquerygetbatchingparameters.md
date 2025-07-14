

- Core Services
- File Metadata
- MDQuery
-  MDQueryGetBatchingParameters(\_:) 

Function

# MDQueryGetBatchingParameters(\_:)

Returns the current parameters that control the batching of progress notifications.

macOS 10.4+

``` source
func MDQueryGetBatchingParameters(_ query: MDQuery!) -> MDQueryBatchingParams
```

## Parameters 

`query`  

The query.

## Return Value

An MDQueryBatchingParams structure with the current batching parameters.

## See Also

### Getting and Setting Query Parameters

func MDQuerySetMaxCount(MDQuery!, CFIndex)

Sets the maximum number of results returned.

func MDQuerySetBatchingParameters(MDQuery!, MDQueryBatchingParams)

Set the query batching parameters.

func MDQueryCopyValueListAttributes(MDQuery!) -> CFArray!

Returns the list of attribute names for which values are being collected by the query.

func MDQueryCopySortingAttributes(MDQuery!) -> CFArray!

Returns the list of attribute names used to sort the results.

func MDQueryCopyQueryString(MDQuery!) -> CFString!

Returns the query string of the query.

