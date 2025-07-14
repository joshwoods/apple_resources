

- Core Services
- File Metadata
- MDQuery
-  MDQueryGetAttributeValueOfResultAtIndex(\_:\_:\_:) 

Function

# MDQueryGetAttributeValueOfResultAtIndex(\_:\_:\_:)

Returns the value of the named attribute for the result at the given index.

macOS 10.4+

``` source
func MDQueryGetAttributeValueOfResultAtIndex(
    _ query: MDQuery!,
    _ name: CFString!,
    _ idx: CFIndex
) -> UnsafeMutableRawPointer!
```

## Parameters 

`query`  

The query.

`name`  

The attribute name to return the values of. If the attribute is not one of those requested in the `valueListAttrs` or `sortingAttrs` parameters to one of the query creation functions, the result will be `NULL`.

`idx`  

The index into the query's result list. If the index is negative or is equal to or larger than the current number of results in the query, the behavior is undefined.

## Return Value

The value of the attribute, or `NULL` if the attribute doesn't exist for the specified result.

## See Also

### Getting Query Result Values

func MDQueryCopyValuesOfAttribute(MDQuery!, CFString!) -> CFArray!

Returns the list of values from the results of the query for the specified attribute.

func MDQueryGetCountOfResultsWithAttributeValue(MDQuery!, CFString!, CFTypeRef!) -> CFIndex

Returns the number of results which have the given attribute and attribute value.

func MDQueryGetIndexOfResult(MDQuery!, UnsafeRawPointer!) -> CFIndex

Returns the current index of the given result.

func MDQueryGetResultAtIndex(MDQuery!, CFIndex) -> UnsafeRawPointer!

Returns the current result at the given index.

func MDQueryGetResultCount(MDQuery!) -> CFIndex

Returns the number of results currently collected by the query.

func MDQuerySetSortComparatorBlock(MDQuery!, ((UnsafePointer&lt;Unmanaged&lt;CFTypeRef>?>?, UnsafePointer&lt;Unmanaged&lt;CFTypeRef>?>?) -> CFComparisonResult)!)

Sets the block used to sort the results of an MDQuery.

