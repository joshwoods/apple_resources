

- Foundation
- NSSortDescriptor
-  init(coder:) 

Initializer

# init(coder:)

Creates a sort descriptor by decoding from the coder you specify.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(coder: NSCoder)
```

## Parameters 

`coder`  

The coder to read data from.

## See Also

### Creating a Sort Descriptor

init(key: String?, ascending: Bool)

Creates a sort descriptor with a specified string key path and sort order.

init(key: String?, ascending: Bool, selector: Selector?)

Creates a sort descriptor with a specified string key path, ordering, and comparison selector.

convenience init&lt;Root, Value>(keyPath: KeyPath&lt;Root, Value>, ascending: Bool)

Creates a sort descriptor with a specified key path and ordering.

init(key: String?, ascending: Bool, comparator: Comparator)

Creates a sort descriptor with a specified string key path and ordering, and a comparator block.

convenience init&lt;Root, Value>(keyPath: KeyPath&lt;Root, Value>, ascending: Bool, comparator: Comparator)

Creates a sort descriptor with a specified key path and ordering, and a comparator block.

convenience init&lt;Compared>(SortDescriptor&lt;Compared>)

Creates a sort descriptor using a sort descriptor you specify.

Deprecated

