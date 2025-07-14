

- Foundation
- NSSortDescriptor
-  selector 

Instance Property

# selector

The selector for comparing objects.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var selector: Selector? { get }
```

## See Also

### Getting Information About a Sort Descriptor

var ascending: Bool

A Boolean value that indicates whether the receiver specifies sorting in ascending order.

var key: String?

The key that specifies the property to compare during sorting.

var keyPath: AnyKeyPath?

The key path that specifies the property to compare during sorting.

var comparator: Comparator

The comparator for the sort descriptor.

