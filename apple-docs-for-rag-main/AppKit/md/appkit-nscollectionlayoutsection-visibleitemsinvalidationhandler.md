

- AppKit
- NSCollectionLayoutSection
-  visibleItemsInvalidationHandler 

Instance Property

# visibleItemsInvalidationHandler

A closure called before each layout cycle to allow modification of the items in the section immediately before they’re displayed.

macOS 10.15+

``` source
@MainActor
var visibleItemsInvalidationHandler: NSCollectionLayoutSectionVisibleItemsInvalidationHandler? { get set }
```

