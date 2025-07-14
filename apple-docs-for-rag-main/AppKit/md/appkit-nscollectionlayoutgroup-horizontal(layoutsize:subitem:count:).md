

- AppKit
- NSCollectionLayoutGroup
-  horizontal(layoutSize:subitem:count:) 

Type Method

# horizontal(layoutSize:subitem:count:)

Creates a group of the specified size, containing an array of equally sized items arranged in a horizontal line up to the number specified by count.

macOS 10.15+

``` source
@MainActor
class func horizontal(
    layoutSize: NSCollectionLayoutSize,
    subitem: NSCollectionLayoutItem,
    count: Int
) -> Self
```

## Discussion

When you set a value for the interItemSpacing property after using this initializer, the group keeps the same number of items and automatically resizes them to add the extra specified spacing between them.

## See Also

### Creating a horizontal group

class func horizontal(layoutSize: NSCollectionLayoutSize, subitems: [NSCollectionLayoutItem]) -> Self

Creates a group of the specified size, containing an array of items arranged in a horizontal line.

