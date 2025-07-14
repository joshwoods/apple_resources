

- UIKit
- NSCollectionLayoutBoundarySupplementaryItem
-  init(layoutSize:elementKind:alignment:absoluteOffset:) 

Initializer

# init(layoutSize:elementKind:alignment:absoluteOffset:)

Creates a boundary supplementary item of the specified size and element kind, with an alignment relative to a section or layout at an absolute offset.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
convenience init(
    layoutSize: NSCollectionLayoutSize,
    elementKind: String,
    alignment: NSRectAlignment,
    absoluteOffset: CGPoint
)
```

## See Also

### Creating a boundary supplementary item

convenience init(layoutSize: NSCollectionLayoutSize, elementKind: String, alignment: NSRectAlignment)

Creates a boundary supplementary item of the specified size and element kind, with an alignment relative to a section or layout.

