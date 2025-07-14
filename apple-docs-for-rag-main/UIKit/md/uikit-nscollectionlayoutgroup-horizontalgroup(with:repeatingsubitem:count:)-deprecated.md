

- UIKit
- NSCollectionLayoutGroup
-  horizontalGroup(with:repeatingSubitem:count:) Deprecated

Type Method

# horizontalGroup(with:repeatingSubitem:count:)

Creates a group that repeats the specified subitem a certain number of times along the horizontal axis.

iOS 16.0–16.0DeprecatediPadOS 16.0–16.0DeprecatedMac CatalysttvOSvisionOS

``` source
@MainActor @preconcurrency
class func horizontalGroup(
    with size: NSCollectionLayoutSize,
    repeatingSubitem subitem: NSCollectionLayoutItem,
    count: Int
) -> NSCollectionLayoutGroup
```

Deprecated

Use horizontal(layoutSize:repeatingSubitem:count:) instead.

## See Also

### Deprecated

class func horizontal(layoutSize: NSCollectionLayoutSize, subitem: NSCollectionLayoutItem, count: Int) -> Self

Creates a group of the specified size, containing an array of equally sized items arranged in a horizontal line up to the number specified by count.

Deprecated

class func vertical(layoutSize: NSCollectionLayoutSize, subitem: NSCollectionLayoutItem, count: Int) -> Self

Creates a group of the specified size, containing an array of equally sized items arranged in a vertical line up to the number specified by count.

Deprecated

class func verticalGroup(with: NSCollectionLayoutSize, repeatingSubitem: NSCollectionLayoutItem, count: Int) -> NSCollectionLayoutGroup

Creates a group that repeats the specified subitem a certain number of times along the vertical axis.

Deprecated

