

- Foundation
- NSSortDescriptor
-  init(key:ascending:selector:) 

Initializer

# init(key:ascending:selector:)

Creates a sort descriptor with a specified string key path, ordering, and comparison selector.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    key: String?,
    ascending: Bool,
    selector: Selector?
)
```

## Parameters 

`key`  

The key path for performing a comparison.

For information about key paths, see Key-Value Coding Programming Guide.

`ascending`  

true if the receiver specifies sorting in ascending order; otherwise, false.

`selector`  

The method to use when comparing the properties of objects, such as localizedStandardCompare(_:). The selector must specify a method that you implement according to the value of the property that the key path identifies. Pass the selector a single parameter, the object to compare against, and it returns the appropriate ComparisonResult constant.

## Return Value

A sort descriptor that initializes with the specified key path, sort order, and comparison selector.

## See Also

### Creating a Sort Descriptor

init(key: String?, ascending: Bool)

Creates a sort descriptor with a specified string key path and sort order.

convenience init&lt;Root, Value>(keyPath: KeyPath&lt;Root, Value>, ascending: Bool)

Creates a sort descriptor with a specified key path and ordering.

init(key: String?, ascending: Bool, comparator: Comparator)

Creates a sort descriptor with a specified string key path and ordering, and a comparator block.

convenience init&lt;Root, Value>(keyPath: KeyPath&lt;Root, Value>, ascending: Bool, comparator: Comparator)

Creates a sort descriptor with a specified key path and ordering, and a comparator block.

init?(coder: NSCoder)

Creates a sort descriptor by decoding from the coder you specify.

convenience init&lt;Compared>(SortDescriptor&lt;Compared>)

Creates a sort descriptor using a sort descriptor you specify.

Deprecated

