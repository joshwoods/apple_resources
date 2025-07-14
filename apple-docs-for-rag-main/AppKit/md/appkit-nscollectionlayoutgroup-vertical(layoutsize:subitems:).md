

- AppKit
- NSCollectionLayoutGroup
-  vertical(layoutSize:subitems:) 

Type Method

# vertical(layoutSize:subitems:)

Creates a group of the specified size, containing an array of items arranged in a vertical line.

macOS 10.15+

``` source
@MainActor
class func vertical(
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

### Creating a vertical group

class func vertical(layoutSize: NSCollectionLayoutSize, subitem: NSCollectionLayoutItem, count: Int) -> Self

Creates a group of the specified size, containing an array of equally sized items arranged in a vertical line up to the number specified by count.

