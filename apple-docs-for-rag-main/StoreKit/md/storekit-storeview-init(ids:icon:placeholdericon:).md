

- StoreKit
- StoreView
-  init(ids:icon:placeholderIcon:) 

Initializer

# init(ids:icon:placeholderIcon:)

Creates a view to load a collection of products from the App Store using product identifiers, and merchandise them using their promotional images and a custom placeholder icon.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
init(
    ids productIDs: some Collection,
    @ViewBuilder icon: @escaping (Product, ProductIconPhase) -> Icon,
    @ViewBuilder placeholderIcon: () -> PlaceholderIcon
)
```

## Parameters 

`productIDs`  

The product identifiers to load from the App Store.

`icon`  

A closure that receives a Product and a ProductIconPhase as input. The ProductIconPhase indicates the state of the loading operation of the product’s promotional image. The closure returns the view to display for the given product and phase value.

`placeholderIcon`  

A closure that returns the view that the store view uses while the products are loading. The store view uses the same placeholder image for all the products.

## Discussion

The store view shows the custom `placeholderIcon` until all products finish loading. After the products finish loading, the view asynchronously loads and displays each product’s promotional image.

Use the ProductIconPhase to monitor the current loading state of a product’s promotional image, and provide a view for each phase. Consider returning the view provided in the `placeholderIcon` closure for during the ProductIconPhase.loading phase. For more information, see ProductIconPhase.

If a product is unavailable, the store view uses the view that the `placeholderIcon` closure provides as a fallback.

## See Also

### Creating store views that load products

init(ids: some Collection&lt;String>, prefersPromotionalIcon: Bool)

Creates a view to load and merchandise a collection of products from the App Store using product identifiers.

init(ids: some Collection&lt;String>, prefersPromotionalIcon: Bool, icon: (Product) -> Icon)

Creates a view to load a collection of products from the App Store using product identifiers, and merchandise them using a custom image.

init(ids: some Collection&lt;String>, prefersPromotionalIcon: Bool, icon: (Product) -> Icon, placeholderIcon: () -> PlaceholderIcon)

Creates a view to load a collection of products from the App Store using product identifiers, and merchandise them using an image and a custom placeholder icon.

