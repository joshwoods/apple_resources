

- Core Services
- File Metadata
- MDQuery
-  MDQueryCreateValueFunction 

Type Alias

# MDQueryCreateValueFunction

Callback function usedto create the value objects stored and returned by a query.

Mac Catalyst 13.0+macOS 10.4+

``` source
typealias MDQueryCreateValueFunction = (MDQuery?, CFString?, CFTypeRef?, UnsafeMutableRawPointer?) -> UnsafeRawPointer?
```

## Parameters 

`query`  

The query instance.

`attrName`  

The attribute name of the value.

`attrValue`  

The default value of the value.

`context`  

The user-defined context parameter provided in the `MDQuerySetCreateValueFunction` function.

## Return Value

The function must return a pointer-sized value that can be managed with the callback which were set at the same time the create function was given to the query. The value must be returned with a reference (such as if the retain callback had been called on it), as implied by the Create name. If this function doesn't wish to create a new object, it can return the given CFTypeRef, but must also return it with a new retain, and the callbacks must be able to handle a `CFTypeRef` as an input value.

## Discussion

The function may hold onto the given attribute name and/or value in some other data structure, but must retain them for them to remain valid

## See Also

### Callbacks

typealias MDQuerySortComparatorFunction

Callback function used to sort the results of a query.

typealias MDQueryCreateResultFunction

Callback function used to create the result objects stored and returned by a query.

