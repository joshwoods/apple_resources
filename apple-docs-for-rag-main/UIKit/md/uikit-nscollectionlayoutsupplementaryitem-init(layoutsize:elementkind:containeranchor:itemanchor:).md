

- UIKit
- NSCollectionLayoutSupplementaryItem
-  init(layoutSize:elementKind:containerAnchor:itemAnchor:) 

Initializer

# init(layoutSize:elementKind:containerAnchor:itemAnchor:)

Creates a supplementary item of the specified size and element kind, an anchor relative to a container, and an anchor relative to an item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
convenience init(
    layoutSize: NSCollectionLayoutSize,
    elementKind: String,
    containerAnchor: NSCollectionLayoutAnchor,
    itemAnchor: NSCollectionLayoutAnchor
)
```

## See Also

### Creating a supplementary item

convenience init(layoutSize: NSCollectionLayoutSize, elementKind: String, containerAnchor: NSCollectionLayoutAnchor)

Creates a supplementary item of the specified size and element kind, with an anchor relative to a container.

