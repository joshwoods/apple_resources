

- Core Services
- File Metadata
- MDQuery
-  MDQueryCopyQueryString(\_:) 

Function

# MDQueryCopyQueryString(\_:)

Returns the query string of the query.

macOS 10.4+

``` source
func MDQueryCopyQueryString(_ query: MDQuery!) -> CFString!
```

## Parameters 

`query`  

The query.

## Return Value

A CFStringRef containing the query string.

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

func MDQueryCopySortingAttributes(MDQuery!) -> CFArray!

Returns the list of attribute names used to sort the results.

