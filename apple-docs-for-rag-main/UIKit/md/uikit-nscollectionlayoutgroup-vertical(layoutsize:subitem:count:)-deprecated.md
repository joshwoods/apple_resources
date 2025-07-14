

- UIKit
- NSCollectionLayoutGroup
-  vertical(layoutSize:subitem:count:) Deprecated

Type Method

# vertical(layoutSize:subitem:count:)

Creates a group of the specified size, containing an array of equally sized items arranged in a vertical line up to the number specified by count.

iOS 13.0–16.0DeprecatediPadOS 13.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedtvOS 13.0–16.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
class func vertical(
    layoutSize: NSCollectionLayoutSize,
    subitem: NSCollectionLayoutItem,
    count: Int
) -> Self
```

Deprecated

Use vertical(layoutSize:repeatingSubitem:count:) instead.

## Discussion

When you set a value for the interItemSpacing property after using this initializer, the group keeps the same number of items and automatically resizes them to add the extra specified spacing between them.

## See Also

### Deprecated

class func horizontal(layoutSize: NSCollectionLayoutSize, subitem: NSCollectionLayoutItem, count: Int) -> Self

Creates a group of the specified size, containing an array of equally sized items arranged in a horizontal line up to the number specified by count.

Deprecated

class func horizontalGroup(with: NSCollectionLayoutSize, repeatingSubitem: NSCollectionLayoutItem, count: Int) -> NSCollectionLayoutGroup

Creates a group that repeats the specified subitem a certain number of times along the horizontal axis.

Deprecated

class func verticalGroup(with: NSCollectionLayoutSize, repeatingSubitem: NSCollectionLayoutItem, count: Int) -> NSCollectionLayoutGroup

Creates a group that repeats the specified subitem a certain number of times along the vertical axis.

Deprecated

