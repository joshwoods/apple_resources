

- UIKit
- NSCollectionLayoutGroup
-  horizontal(layoutSize:repeatingSubitem:count:) 

Type Method

# horizontal(layoutSize:repeatingSubitem:count:)

Creates a group that repeats the specified subitem a certain number of times along the horizontal axis.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
@MainActor
class func horizontal(
    layoutSize: NSCollectionLayoutSize,
    repeatingSubitem subitem: NSCollectionLayoutItem,
    count: Int
) -> Self
```

## Parameters 

`layoutSize`  

The group’s size.

`subitem`  

The subitem to repeat. It’s your responsibility to ensure that the group’s `layoutSize` can fit `count` repetitions of this item.

`count`  

The number of times to repeat the subitem.

## See Also

### Creating a horizontal group

class func horizontal(layoutSize: NSCollectionLayoutSize, subitems: [NSCollectionLayoutItem]) -> Self

Creates a group of the specified size, containing an array of items arranged in a horizontal line.

