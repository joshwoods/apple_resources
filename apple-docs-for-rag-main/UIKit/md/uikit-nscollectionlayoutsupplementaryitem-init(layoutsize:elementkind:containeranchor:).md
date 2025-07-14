

- UIKit
- NSCollectionLayoutSupplementaryItem
-  init(layoutSize:elementKind:containerAnchor:) 

Initializer

# init(layoutSize:elementKind:containerAnchor:)

Creates a supplementary item of the specified size and element kind, with an anchor relative to a container.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
convenience init(
    layoutSize: NSCollectionLayoutSize,
    elementKind: String,
    containerAnchor: NSCollectionLayoutAnchor
)
```

## See Also

### Creating a supplementary item

convenience init(layoutSize: NSCollectionLayoutSize, elementKind: String, containerAnchor: NSCollectionLayoutAnchor, itemAnchor: NSCollectionLayoutAnchor)

Creates a supplementary item of the specified size and element kind, an anchor relative to a container, and an anchor relative to an item.

