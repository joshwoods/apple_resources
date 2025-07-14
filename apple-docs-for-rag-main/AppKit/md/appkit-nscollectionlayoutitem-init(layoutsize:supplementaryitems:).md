

- AppKit
- NSCollectionLayoutItem
-  init(layoutSize:supplementaryItems:) 

Initializer

# init(layoutSize:supplementaryItems:)

Creates an item of the specified size with an array of supplementary items to attach to the item.

macOS 10.15+

``` source
@MainActor
convenience init(
    layoutSize: NSCollectionLayoutSize,
    supplementaryItems: [NSCollectionLayoutSupplementaryItem]
)
```

## See Also

### Creating an item

convenience init(layoutSize: NSCollectionLayoutSize)

Creates an item of the specified size.

