

- Core Services
- File Metadata
- MDQuery
-  MDQueryGetResultAtIndex(\_:\_:) 

Function

# MDQueryGetResultAtIndex(\_:\_:)

Returns the current result at the given index.

macOS 10.4+

``` source
func MDQueryGetResultAtIndex(
    _ query: MDQuery!,
    _ idx: CFIndex
) -> UnsafeRawPointer!
```

## Parameters 

`query`  

The query.

`idx`  

The index into the query's result list. If the index is negative, or is equal to or larger than the current number of results in the query, the behavior is undefined.

## Return Value

Returns the MDItemRef currently at the given index, or if a result-creation function has been set, returns the result returned by that function.

## Discussion

This function causes the result object to be created if it hasn't been created already. For performance reasons you should only request objects that you require. If possible, call this function to fetch only the results you need to display or otherwise process.

Note that the index of a particular result can change over time if the query is configured to allow live-updates.

## See Also

### Getting Query Result Values

func MDQueryCopyValuesOfAttribute(MDQuery!, CFString!) -> CFArray!

Returns the list of values from the results of the query for the specified attribute.

func MDQueryGetAttributeValueOfResultAtIndex(MDQuery!, CFString!, CFIndex) -> UnsafeMutableRawPointer!

Returns the value of the named attribute for the result at the given index.

func MDQueryGetCountOfResultsWithAttributeValue(MDQuery!, CFString!, CFTypeRef!) -> CFIndex

Returns the number of results which have the given attribute and attribute value.

func MDQueryGetIndexOfResult(MDQuery!, UnsafeRawPointer!) -> CFIndex

Returns the current index of the given result.

func MDQueryGetResultCount(MDQuery!) -> CFIndex

Returns the number of results currently collected by the query.

func MDQuerySetSortComparatorBlock(MDQuery!, ((UnsafePointer&lt;Unmanaged&lt;CFTypeRef>?>?, UnsafePointer&lt;Unmanaged&lt;CFTypeRef>?>?) -> CFComparisonResult)!)

Sets the block used to sort the results of an MDQuery.

