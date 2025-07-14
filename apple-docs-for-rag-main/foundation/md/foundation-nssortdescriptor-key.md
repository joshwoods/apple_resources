

- Foundation
- NSSortDescriptor
-  key 

Instance Property

# key

The key that specifies the property to compare during sorting.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var key: String? { get }
```

## See Also

### Getting Information About a Sort Descriptor

var ascending: Bool

A Boolean value that indicates whether the receiver specifies sorting in ascending order.

var keyPath: AnyKeyPath?

The key path that specifies the property to compare during sorting.

var selector: Selector?

The selector for comparing objects.

var comparator: Comparator

The comparator for the sort descriptor.

