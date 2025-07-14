

- UIKit
- NSCollectionLayoutGroup
-  horizontal(layoutSize:subitems:) 

Type Method

# horizontal(layoutSize:subitems:)

Creates a group of the specified size, containing an array of items arranged in a horizontal line.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

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

class func horizontal(layoutSize: NSCollectionLayoutSize, repeatingSubitem: NSCollectionLayoutItem, count: Int) -> Self

Creates a group that repeats the specified subitem a certain number of times along the horizontal axis.

