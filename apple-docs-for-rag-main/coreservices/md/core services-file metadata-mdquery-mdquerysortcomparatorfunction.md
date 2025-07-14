

- Core Services
- File Metadata
- MDQuery
-  MDQuerySortComparatorFunction 

Type Alias

# MDQuerySortComparatorFunction

Callback function used to sort the results of a query.

Mac Catalyst 13.0+macOS 10.4+

``` source
typealias MDQuerySortComparatorFunction = (UnsafePointer?>?, UnsafePointer?>?, UnsafeMutableRawPointer?) -> CFComparisonResult
```

## Parameters 

`query`  

The query instance.

`attrs1`  

A C array of attribute values for a result. The values occur in the array in the same order and position that the attribute names were passed in the `sortingAttrs` array when the query was created. The values of the attributes will be `NULL` if the attribute doesn't exist for a result or if read access to that attribute is not allowed.

`attrs2`  

A C array of attribute values for a result. The values occur in the array in the same order and position that the attribute names were passed in the `sortingAttrs` array when the query was created. The values of the attributes will be `NULL` if the attribute doesn't exist for a result or if read access to that attribute is not allowed.

`context`  

The user-defined context parameter provided in the function `MDQuerySetSortComparator`.

## Return Value

The function must return one of the CFComparisonResults `kCFCompareLessThan`, `kCFCompareEqualTo`, or `kCFCompareGreaterThan`. There is no provision for unordered results. The comparison should be a total order relation and produce the same results for the same inputs.

## See Also

### Callbacks

typealias MDQueryCreateResultFunction

Callback function used to create the result objects stored and returned by a query.

typealias MDQueryCreateValueFunction

Callback function usedto create the value objects stored and returned by a query.

