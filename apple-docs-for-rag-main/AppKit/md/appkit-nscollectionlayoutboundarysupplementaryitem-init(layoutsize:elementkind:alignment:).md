

- AppKit
- NSCollectionLayoutBoundarySupplementaryItem
-  init(layoutSize:elementKind:alignment:) 

Initializer

# init(layoutSize:elementKind:alignment:)

Creates a boundary supplementary item of the specified size and element kind, with an alignment relative to a section or layout.

macOS 10.15+

``` source
@MainActor
convenience init(
    layoutSize: NSCollectionLayoutSize,
    elementKind: String,
    alignment: NSRectAlignment
)
```

## See Also

### Creating a boundary supplementary item

convenience init(layoutSize: NSCollectionLayoutSize, elementKind: String, alignment: NSRectAlignment, absoluteOffset: NSPoint)

Creates a boundary supplementary item of the specified size and element kind, with an alignment relative to a section or layout at an absolute offset.

