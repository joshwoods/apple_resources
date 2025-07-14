

- AppKit
- NSCollectionLayoutGroup
-  custom(layoutSize:itemProvider:) 

Type Method

# custom(layoutSize:itemProvider:)

Creates a group of the specified size, with an item provider that creates a custom arrangement for those items.

macOS 10.15+

``` source
@MainActor
class func custom(
    layoutSize: NSCollectionLayoutSize,
    itemProvider: @escaping NSCollectionLayoutGroupCustomItemProvider
) -> Self
```

