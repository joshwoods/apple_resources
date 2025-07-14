

- AppKit
- NSCollectionLayoutBoundarySupplementaryItem
-  init(layoutSize:elementKind:alignment:absoluteOffset:) 

Initializer

# init(layoutSize:elementKind:alignment:absoluteOffset:)

Creates a boundary supplementary item of the specified size and element kind, with an alignment relative to a section or layout at an absolute offset.

macOS 10.15+

``` source
@MainActor
convenience init(
    layoutSize: NSCollectionLayoutSize,
    elementKind: String,
    alignment: NSRectAlignment,
    absoluteOffset: NSPoint
)
```

## See Also

### Creating a boundary supplementary item

convenience init(layoutSize: NSCollectionLayoutSize, elementKind: String, alignment: NSRectAlignment)

Creates a boundary supplementary item of the specified size and element kind, with an alignment relative to a section or layout.

