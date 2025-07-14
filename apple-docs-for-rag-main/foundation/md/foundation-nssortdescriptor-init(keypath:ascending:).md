

- Foundation
- NSSortDescriptor
-  init(keyPath:ascending:) 

Initializer

# init(keyPath:ascending:)

Creates a sort descriptor with a specified key path and ordering.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(
    keyPath: KeyPath,
    ascending: Bool
)
```

## Parameters 

`keyPath`  

The key path to the property to compare.

`ascending`  

If `true`, the sort descriptor compares using the SortOrder.forward sort order; otherwise, it uses SortOrder.reverse.

## See Also

### Creating a Sort Descriptor

init(key: String?, ascending: Bool)

Creates a sort descriptor with a specified string key path and sort order.

init(key: String?, ascending: Bool, selector: Selector?)

Creates a sort descriptor with a specified string key path, ordering, and comparison selector.

init(key: String?, ascending: Bool, comparator: Comparator)

Creates a sort descriptor with a specified string key path and ordering, and a comparator block.

convenience init&lt;Root, Value>(keyPath: KeyPath&lt;Root, Value>, ascending: Bool, comparator: Comparator)

Creates a sort descriptor with a specified key path and ordering, and a comparator block.

init?(coder: NSCoder)

Creates a sort descriptor by decoding from the coder you specify.

convenience init&lt;Compared>(SortDescriptor&lt;Compared>)

Creates a sort descriptor using a sort descriptor you specify.

Deprecated

