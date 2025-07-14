

- Core Services
- File Metadata
- MDQuery
-  MDQueryGetIndexOfResult(\_:\_:) 

Function

# MDQueryGetIndexOfResult(\_:\_:)

Returns the current index of the given result.

macOS 10.4+

``` source
func MDQueryGetIndexOfResult(
    _ query: MDQuery!,
    _ result: UnsafeRawPointer!
) -> CFIndex
```

## Parameters 

`query`  

The query.

`result`  

The result object to search for. If a custom create-result function has been set and this parameter is not a valid result object that the provided callbacks can handle, the behavior is undefined. If a custom create-result function has not been set this parameter must be a valid MDItemRef.

## Return Value

The index of the given result, or `kCFNotFound` if the value is not one of the query's existing results. If you provided a custom result creation function result, the result will be objects created by that function.

## Discussion

If a result-create function has been set, and the equal callback is non-`NULL`, it will be used to test the query's results against the candidate result.

Note that the index of a result can change over time if the query allows live-updates.

## See Also

### Getting Query Result Values

func MDQueryCopyValuesOfAttribute(MDQuery!, CFString!) -> CFArray!

Returns the list of values from the results of the query for the specified attribute.

func MDQueryGetAttributeValueOfResultAtIndex(MDQuery!, CFString!, CFIndex) -> UnsafeMutableRawPointer!

Returns the value of the named attribute for the result at the given index.

func MDQueryGetCountOfResultsWithAttributeValue(MDQuery!, CFString!, CFTypeRef!) -> CFIndex

Returns the number of results which have the given attribute and attribute value.

func MDQueryGetResultAtIndex(MDQuery!, CFIndex) -> UnsafeRawPointer!

Returns the current result at the given index.

func MDQueryGetResultCount(MDQuery!) -> CFIndex

Returns the number of results currently collected by the query.

func MDQuerySetSortComparatorBlock(MDQuery!, ((UnsafePointer&lt;Unmanaged&lt;CFTypeRef>?>?, UnsafePointer&lt;Unmanaged&lt;CFTypeRef>?>?) -> CFComparisonResult)!)

Sets the block used to sort the results of an MDQuery.

