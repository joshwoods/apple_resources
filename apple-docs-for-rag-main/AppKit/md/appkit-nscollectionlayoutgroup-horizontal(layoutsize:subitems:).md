

- AppKit
- NSCollectionLayoutGroup
-  horizontal(layoutSize:subitems:) 

Type Method

# horizontal(layoutSize:subitems:)

Creates a group of the specified size, containing an array of items arranged in a horizontal line.

macOS 10.15+

``` source
@MainActor
class func horizontal(
    layoutSize: NSCollectionLayoutSize,
    subitems: [NSCollectionLayoutItem]
) -> Self
```

## Parameters 

`layoutSize`  

The group’s size.

`subitems`  

The subitems to include.

## See Also

### Creating a horizontal group

class func horizontal(layoutSize: NSCollectionLayoutSize, subitem: NSCollectionLayoutItem, count: Int) -> Self

Creates a group of the specified size, containing an array of equally sized items arranged in a horizontal line up to the number specified by count.

