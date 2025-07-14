

- Core Services
- File Metadata
- MDQuery
-  MDQueryGetCountOfResultsWithAttributeValue(\_:\_:\_:) 

Function

# MDQueryGetCountOfResultsWithAttributeValue(\_:\_:\_:)

Returns the number of results which have the given attribute and attribute value.

macOS 10.4+

``` source
func MDQueryGetCountOfResultsWithAttributeValue(
    _ query: MDQuery!,
    _ name: CFString!,
    _ value: CFTypeRef!
) -> CFIndex
```

## Parameters 

`query`  

The query.

`name`  

The attribute name to return the result count of. If the attribute is not one of those requested in the `valueListAttrs` parameter, the behavior is undefined.

`value`  

The attribute value for which to return the number of results with that value. This parameter may be `NULL`, in which case the number of results that do not contain the specified attribute is returned.

## Return Value

The number of results containing that attribute and value.

## Discussion

This count may change over time if the query allows live-updates.

## See Also

### Getting Query Result Values

func MDQueryCopyValuesOfAttribute(MDQuery!, CFString!) -> CFArray!

Returns the list of values from the results of the query for the specified attribute.

func MDQueryGetAttributeValueOfResultAtIndex(MDQuery!, CFString!, CFIndex) -> UnsafeMutableRawPointer!

Returns the value of the named attribute for the result at the given index.

func MDQueryGetIndexOfResult(MDQuery!, UnsafeRawPointer!) -> CFIndex

Returns the current index of the given result.

func MDQueryGetResultAtIndex(MDQuery!, CFIndex) -> UnsafeRawPointer!

Returns the current result at the given index.

func MDQueryGetResultCount(MDQuery!) -> CFIndex

Returns the number of results currently collected by the query.

func MDQuerySetSortComparatorBlock(MDQuery!, ((UnsafePointer&lt;Unmanaged&lt;CFTypeRef>?>?, UnsafePointer&lt;Unmanaged&lt;CFTypeRef>?>?) -> CFComparisonResult)!)

Sets the block used to sort the results of an MDQuery.

