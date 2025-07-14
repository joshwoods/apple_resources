

- Foundation
- NSSortDescriptor
-  comparator 

Instance Property

# comparator

The comparator for the sort descriptor.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var comparator: Comparator { get }
```

## Discussion

Call this property only for sort descriptors initialized with init(key:ascending:comparator:).

## See Also

### Getting Information About a Sort Descriptor

var ascending: Bool

A Boolean value that indicates whether the receiver specifies sorting in ascending order.

var key: String?

The key that specifies the property to compare during sorting.

var keyPath: AnyKeyPath?

The key path that specifies the property to compare during sorting.

var selector: Selector?

The selector for comparing objects.

