

- Foundation
- NSSortDescriptor
-  init(\_:) Deprecated

Initializer

# init(\_:)

Creates a sort descriptor using a sort descriptor you specify.

iOS 15.0–17.0DeprecatediPadOS 15.0–17.0DeprecatedMac Catalyst 15.0–17.0DeprecatedmacOS 12.0–14.0DeprecatedtvOS 15.0–17.0DeprecatedvisionOS 1.0+watchOS 8.0–10.0Deprecated

``` source
convenience init(_ sortDescriptor: SortDescriptor)
```

Deprecated

Use \`init(\_:) where Compared: NSObject\` instead. Attempt to convert SortDescriptor with Compared being non-NSObject will result in a fatalError at runtime.

## Parameters 

`sortDescriptor`  

A sort descriptor.

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

init?(coder: NSCoder)

Creates a sort descriptor by decoding from the coder you specify.

