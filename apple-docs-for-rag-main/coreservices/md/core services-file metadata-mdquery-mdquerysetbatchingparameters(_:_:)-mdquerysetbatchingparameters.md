

- Core Services
- File Metadata
- MDQuery
-  MDQuerySetBatchingParameters(\_:\_:) 

Function

# MDQuerySetBatchingParameters(\_:\_:)

Set the query batching parameters.

macOS 10.4+

``` source
func MDQuerySetBatchingParameters(
    _ query: MDQuery!,
    _ params: MDQueryBatchingParams
)
```

## Parameters 

`query`  

The query.

`params`  

An MDQueryBatchingParams structure with the batching parameters to set.

## See Also

### Getting and Setting Query Parameters

func MDQuerySetMaxCount(MDQuery!, CFIndex)

Sets the maximum number of results returned.

func MDQueryGetBatchingParameters(MDQuery!) -> MDQueryBatchingParams

Returns the current parameters that control the batching of progress notifications.

func MDQueryCopyValueListAttributes(MDQuery!) -> CFArray!

Returns the list of attribute names for which values are being collected by the query.

func MDQueryCopySortingAttributes(MDQuery!) -> CFArray!

Returns the list of attribute names used to sort the results.

func MDQueryCopyQueryString(MDQuery!) -> CFString!

Returns the query string of the query.

