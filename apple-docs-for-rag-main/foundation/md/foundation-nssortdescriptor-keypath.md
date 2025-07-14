

- Foundation
- NSSortDescriptor
-  keyPath 

Instance Property

# keyPath

The key path that specifies the property to compare during sorting.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var keyPath: AnyKeyPath? { get }
```

## See Also

### Getting Information About a Sort Descriptor

var ascending: Bool

A Boolean value that indicates whether the receiver specifies sorting in ascending order.

var key: String?

The key that specifies the property to compare during sorting.

var selector: Selector?

The selector for comparing objects.

var comparator: Comparator

The comparator for the sort descriptor.

