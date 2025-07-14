

- Core Services
- File Metadata
- MDQuery
-  MDQuerySetSortComparator(\_:\_:\_:) 

Function

# MDQuerySetSortComparator(\_:\_:\_:)

Sets the function used to sort the results of an MDQuery.

macOS 10.4+

``` source
func MDQuerySetSortComparator(
    _ query: MDQuery!,
    _ comparator: MDQuerySortComparatorFunction!,
    _ context: UnsafeMutableRawPointer!
)
```

## Parameters 

`query`  

The query.

`comparator`  

The callback function the MDQuery uses to sort the results list. This parameter may be `NULL` which cancels previous sort comparator settings. If a function is specified and is not of type `MDQuerySortComparatorFunction` or does not behave as a `MDQuerySortComparatorFunction` must, the behavior is undefined.

`context`  

A pointer-sized user-defined value, that is passed as the third parameter to the create function. MDQuery does not use this value, does not retain the context in any way, and requires that the context be valid for the lifetime of the query. If the context is not what is expected by the create function, the behavior is undefined.

## See Also

### Setting Callback Functions

func MDQuerySetCreateResultFunction(MDQuery!, MDQueryCreateResultFunction!, UnsafeMutableRawPointer!, UnsafePointer&lt;CFArrayCallBacks>!)

Sets the function used to create the result objects of the MDQuery.

func MDQuerySetCreateValueFunction(MDQuery!, MDQueryCreateValueFunction!, UnsafeMutableRawPointer!, UnsafePointer&lt;CFArrayCallBacks>!)

Sets the function used to create the value objects of the MDQuery.

