

- Foundation
- NSSortDescriptor
-  init(key:ascending:comparator:) 

Initializer

# init(key:ascending:comparator:)

Creates a sort descriptor with a specified string key path and ordering, and a comparator block.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    key: String?,
    ascending: Bool,
    comparator cmptr: @escaping Comparator
)
```

## Parameters 

`key`  

The property key for performing a comparison.

For information about key paths, see Key-Value Coding Programming Guide.

`ascending`  

true if the receiver specifies sorting in ascending order; otherwise, false.

`cmptr`  

A comparator block.

## Return Value

A sort descriptor that initializes with the specified key, ordering, and comparator.

## See Also

### Creating a Sort Descriptor

init(key: String?, ascending: Bool)

Creates a sort descriptor with a specified string key path and sort order.

init(key: String?, ascending: Bool, selector: Selector?)

Creates a sort descriptor with a specified string key path, ordering, and comparison selector.

convenience init&lt;Root, Value>(keyPath: KeyPath&lt;Root, Value>, ascending: Bool)

Creates a sort descriptor with a specified key path and ordering.

convenience init&lt;Root, Value>(keyPath: KeyPath&lt;Root, Value>, ascending: Bool, comparator: Comparator)

Creates a sort descriptor with a specified key path and ordering, and a comparator block.

init?(coder: NSCoder)

Creates a sort descriptor by decoding from the coder you specify.

convenience init&lt;Compared>(SortDescriptor&lt;Compared>)

Creates a sort descriptor using a sort descriptor you specify.

Deprecated

