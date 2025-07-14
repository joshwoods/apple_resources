

- Core Services
- File Metadata
- MDQuery
-  MDQueryGetResultCount(\_:) 

Function

# MDQueryGetResultCount(\_:)

Returns the number of results currently collected by the query.

macOS 10.4+

``` source
func MDQueryGetResultCount(_ query: MDQuery!) -> CFIndex
```

## Parameters 

`query`  

The query.

## Return Value

The number of results in the query.

## Discussion

Note that the number of results in a query will change over time as the query's result list is updated.

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

func MDQueryGetResultAtIndex(MDQuery!, CFIndex) -> UnsafeRawPointer!

Returns the current result at the given index.

func MDQuerySetSortComparatorBlock(MDQuery!, ((UnsafePointer&lt;Unmanaged&lt;CFTypeRef>?>?, UnsafePointer&lt;Unmanaged&lt;CFTypeRef>?>?) -> CFComparisonResult)!)

Sets the block used to sort the results of an MDQuery.

