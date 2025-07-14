

- Core Services
- File Metadata
- MDQuery
-  MDQueryCopyValuesOfAttribute(\_:\_:) 

Function

# MDQueryCopyValuesOfAttribute(\_:\_:)

Returns the list of values from the results of the query for the specified attribute.

macOS 10.4+

``` source
func MDQueryCopyValuesOfAttribute(
    _ query: MDQuery!,
    _ name: CFString!
) -> CFArray!
```

## Parameters 

`query`  

The query.

`name`  

The attribute name to return the value of. If the attribute is not one of those requested when the query was created the behavior is undefined

## Return Value

A CFArrayRef containing the value objects for the specified attribute. The array contents are not ordered and contain only one occurrence of each value. The array contents may change over time if the query is configured for live-updates.

## See Also

### Getting Query Result Values

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

func MDQuerySetSortComparatorBlock(MDQuery!, ((UnsafePointer&lt;Unmanaged&lt;CFTypeRef>?>?, UnsafePointer&lt;Unmanaged&lt;CFTypeRef>?>?) -> CFComparisonResult)!)

Sets the block used to sort the results of an MDQuery.

