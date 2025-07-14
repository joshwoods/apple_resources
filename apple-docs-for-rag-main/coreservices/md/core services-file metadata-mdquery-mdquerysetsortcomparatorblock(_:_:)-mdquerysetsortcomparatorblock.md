

- Core Services
- File Metadata
- MDQuery
-  MDQuerySetSortComparatorBlock(\_:\_:) 

Function

# MDQuerySetSortComparatorBlock(\_:\_:)

Sets the block used to sort the results of an MDQuery.

macOS 10.6+

``` source
func MDQuerySetSortComparatorBlock(
    _ query: MDQuery!,
    _ comparator: ((UnsafePointer?>?, UnsafePointer?>?) -> CFComparisonResult)!
)
```

## Parameters 

`query`  

The query.

`comparator`  

The callback block the MDQuery will use to sort its results. The comparator may be called on multiple threads in parallel, and must be reentrant. To take advantage of parallel sorting, it is best to avoid any locking in the comparator.

The block may be `NULL` to cancel any custom comparator.

## Discussion

You may set the comparator block as many times as you like, even while the query is executing. Whenever the comparator block is set, all results are re-sorted using the new comparator block before the function returns. The block can be NULL to cancel custom sorting and revert to the default sorting.

The default sort provided by MDQueryCreate(_:_:_:_:) is an ascending sort. Strings are compared using CFStringCompare(_:_:_:) with the options compareNonliteral \| compareLocalized \| compareNumerically. `CFDataRefs` are compared by using `memcmp()` of the data pointers.

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

func MDQueryGetResultCount(MDQuery!) -> CFIndex

Returns the number of results currently collected by the query.

