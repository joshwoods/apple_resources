

- StoreKit
- StoreView
-  init(ids:prefersPromotionalIcon:icon:) 

Initializer

# init(ids:prefersPromotionalIcon:icon:)

Creates a view to load a collection of products from the App Store using product identifiers, and merchandise them using a custom image.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
init(
    ids productIDs: some Collection,
    prefersPromotionalIcon: Bool = false,
    @ViewBuilder icon: @escaping (Product) -> Icon
) where PlaceholderIcon == AutomaticProductPlaceholderIcon
```

## Parameters 

`productIDs`  

The product identifiers to load from the App Store.

`prefersPromotionalIcon`  

A Boolean value that indicates whether to use promotional images from the App Store, if they’re available. If this parameter is `false`, the system ignores promotional images.

`icon`  

A closure that returns the image the view displays when the products finish loading from the App Store.

## Discussion

The store view shows a placeholder icon until all products finish loading. Then, the view uses the image that you provide in `icon`, by default. If you set `prefersPromotionalIcon` to `true`, the view uses the promotional image instead of the `icon` for any products that have promotional images available.

## See Also

### Creating store views that load products

init(ids: some Collection&lt;String>, prefersPromotionalIcon: Bool)

Creates a view to load and merchandise a collection of products from the App Store using product identifiers.

init(ids: some Collection&lt;String>, prefersPromotionalIcon: Bool, icon: (Product) -> Icon, placeholderIcon: () -> PlaceholderIcon)

Creates a view to load a collection of products from the App Store using product identifiers, and merchandise them using an image and a custom placeholder icon.

init(ids: some Collection&lt;String>, icon: (Product, ProductIconPhase) -> Icon, placeholderIcon: () -> PlaceholderIcon)

Creates a view to load a collection of products from the App Store using product identifiers, and merchandise them using their promotional images and a custom placeholder icon.

