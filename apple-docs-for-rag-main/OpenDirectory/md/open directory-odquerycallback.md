

- Open Directory
-  ODQueryCallback 

Type Alias

# ODQueryCallback

A callback function called as results from a scheduled query are returned.

Mac CatalystmacOS

``` source
typealias ODQueryCallback = (ODQueryRef?, CFArray?, CFError?, UnsafeMutableRawPointer?) -> Void
```

## Discussion

Results from this function must be retained or copied. The results from any given call are partial. If both `inResults` and `inError` are `NULL`, the query has completed.

## See Also

### Data Types

typealias ODAttributeType

An Open Directory attribute type.

typealias ODAuthenticationType

An Open Directory authentication type.

class ODContext

An Open Directory context type.

class ODNodeRef

An Open Directory node type.

class ODQueryRef

An Open Directory query type.

class ODRecordRef

An Open Directory record type.

class ODSessionRef

An Open Directory session type.

typealias ODMatchType

An Open Directory match type.

typealias ODNodeType

An Open Directory node type.

typealias ODRecordType

An Open Directory record type.

\_ODAttributeType

An Open Directory attribute type.

\_ODAuthenticationType

An Open Directory authentication type.

\_ODRecordType

An Open Directory record type.

