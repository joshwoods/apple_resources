

- AppKit
- NSCollectionLayoutAnchor
-  isAbsoluteOffset 

Instance Property

# isAbsoluteOffset

A Boolean value that indicates whether the anchor’s offset is expressed as an absolute value.

macOS 10.15+

``` source
@MainActor
var isAbsoluteOffset: Bool { get }
```

## See Also

### Getting the offset

var offset: NSPoint

The floating-point value of the anchor’s offset from the item it’s attached to.

var isFractionalOffset: Bool

A Boolean value that indicates whether the anchor’s offset is expressed as a fraction of its supplementary item’s dimension.

