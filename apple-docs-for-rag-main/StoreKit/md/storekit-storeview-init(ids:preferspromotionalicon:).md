

- StoreKit
- StoreView
-  init(ids:prefersPromotionalIcon:) 

Initializer

# init(ids:prefersPromotionalIcon:)

Creates a view to load and merchandise a collection of products from the App Store using product identifiers.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
init(
    ids productIDs: some Collection,
    prefersPromotionalIcon: Bool = false
) where Icon == EmptyView, PlaceholderIcon == EmptyView
```

## Parameters 

`productIDs`  

The product identifiers to load from the App Store.

`prefersPromotionalIcon`  

A Boolean value that indicates whether to use promotional images from the App Store, if they’re available. If this parameter is `false`, the system ignores promotional images.

## See Also

### Creating store views that load products

init(ids: some Collection&lt;String>, prefersPromotionalIcon: Bool, icon: (Product) -> Icon)

Creates a view to load a collection of products from the App Store using product identifiers, and merchandise them using a custom image.

init(ids: some Collection&lt;String>, prefersPromotionalIcon: Bool, icon: (Product) -> Icon, placeholderIcon: () -> PlaceholderIcon)

Creates a view to load a collection of products from the App Store using product identifiers, and merchandise them using an image and a custom placeholder icon.

init(ids: some Collection&lt;String>, icon: (Product, ProductIconPhase) -> Icon, placeholderIcon: () -> PlaceholderIcon)

Creates a view to load a collection of products from the App Store using product identifiers, and merchandise them using their promotional images and a custom placeholder icon.

