

- UIKit
- NSCollectionLayoutGroup
-  custom(layoutSize:itemProvider:) 

Type Method

# custom(layoutSize:itemProvider:)

Creates a group of the specified size, with an item provider that creates a custom arrangement for those items.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class func custom(
    layoutSize: NSCollectionLayoutSize,
    itemProvider: @escaping NSCollectionLayoutGroupCustomItemProvider
) -> Self
```

