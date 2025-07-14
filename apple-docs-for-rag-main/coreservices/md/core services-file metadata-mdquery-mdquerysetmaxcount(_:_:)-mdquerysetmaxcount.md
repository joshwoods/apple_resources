

- Core Services
- File Metadata
- MDQuery
-  MDQuerySetMaxCount(\_:\_:) 

Function

# MDQuerySetMaxCount(\_:\_:)

Sets the maximum number of results returned.

macOS 10.5+

``` source
func MDQuerySetMaxCount(
    _ query: MDQuery!,
    _ size: CFIndex
)
```

## Parameters 

`query`  

The query.

`size`  

The maximum number of return results.

## Discussion

This must be called before the query is executed.

## See Also

### Getting and Setting Query Parameters

func MDQueryGetBatchingParameters(MDQuery!) -> MDQueryBatchingParams

Returns the current parameters that control the batching of progress notifications.

func MDQuerySetBatchingParameters(MDQuery!, MDQueryBatchingParams)

Set the query batching parameters.

func MDQueryCopyValueListAttributes(MDQuery!) -> CFArray!

Returns the list of attribute names for which values are being collected by the query.

func MDQueryCopySortingAttributes(MDQuery!) -> CFArray!

Returns the list of attribute names used to sort the results.

func MDQueryCopyQueryString(MDQuery!) -> CFString!

Returns the query string of the query.

