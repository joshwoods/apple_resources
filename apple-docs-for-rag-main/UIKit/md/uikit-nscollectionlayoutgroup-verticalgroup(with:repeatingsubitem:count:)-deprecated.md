

- UIKit
- NSCollectionLayoutGroup
-  verticalGroup(with:repeatingSubitem:count:) Deprecated

Type Method

# verticalGroup(with:repeatingSubitem:count:)

Creates a group that repeats the specified subitem a certain number of times along the vertical axis.

iOS 16.0–16.0DeprecatediPadOS 16.0–16.0DeprecatedMac CatalysttvOSvisionOS

``` source
@MainActor @preconcurrency
class func verticalGroup(
    with size: NSCollectionLayoutSize,
    repeatingSubitem subitem: NSCollectionLayoutItem,
    count: Int
) -> NSCollectionLayoutGroup
```

Deprecated

Use vertical(layoutSize:repeatingSubitem:count:) instead.

## See Also

### Deprecated

class func horizontal(layoutSize: NSCollectionLayoutSize, subitem: NSCollectionLayoutItem, count: Int) -> Self

Creates a group of the specified size, containing an array of equally sized items arranged in a horizontal line up to the number specified by count.

Deprecated

class func horizontalGroup(with: NSCollectionLayoutSize, repeatingSubitem: NSCollectionLayoutItem, count: Int) -> NSCollectionLayoutGroup

Creates a group that repeats the specified subitem a certain number of times along the horizontal axis.

Deprecated

class func vertical(layoutSize: NSCollectionLayoutSize, subitem: NSCollectionLayoutItem, count: Int) -> Self

Creates a group of the specified size, containing an array of equally sized items arranged in a vertical line up to the number specified by count.

Deprecated

