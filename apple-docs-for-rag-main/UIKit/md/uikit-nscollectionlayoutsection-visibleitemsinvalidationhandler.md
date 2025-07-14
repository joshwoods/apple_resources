

- UIKit
- NSCollectionLayoutSection
-  visibleItemsInvalidationHandler 

Instance Property

# visibleItemsInvalidationHandler

A closure called before each layout cycle to allow modification of the items in the section immediately before they’re displayed.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var visibleItemsInvalidationHandler: NSCollectionLayoutSectionVisibleItemsInvalidationHandler? { get set }
```

