

- StoreKit
- StoreView
-  init(ids:prefersPromotionalIcon:icon:placeholderIcon:) 

Initializer

# init(ids:prefersPromotionalIcon:icon:placeholderIcon:)

Creates a view to load a collection of products from the App Store using product identifiers, and merchandise them using an image and a custom placeholder icon.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
init(
    ids productIDs: some Collection,
    prefersPromotionalIcon: Bool = false,
    @ViewBuilder icon: @escaping (Product) -> Icon,
    @ViewBuilder placeholderIcon: () -> PlaceholderIcon
)
```

## Parameters 

`productIDs`  

The product identifiers to load from the App Store.

`prefersPromotionalIcon`  

A Boolean value that indicates whether to use a promotional image from the App Store, if it’s available. If this parameter is `false`, the system ignores promotional images.

`icon`  

A closure that returns the image the view displays when the products finish loading from the App Store.

`placeholderIcon`  

A closure that returns the image that the view uses while the products are loading. The view uses the same placeholder image for all the products.

## Discussion

The store view shows the custom placeholder icon until all products finish loading. After the view finishes loading the products, it uses the image you provide, by default. If you set `prefersPromotionalIcon` to `true`, any products that have an available promotional image use the promotional image instead.

The following example shows how to create a store view using an icon and a custom placeholder icon:

```
StoreView(ids: [
    "com.example.product1",
    "com.example.product2"
]) { product in
     Image(systemName: "star.fill")
         .foregroundStyle(.yellow)
 } placeholderIcon: {
      Image(systemName: "star.fill")
         .foregroundStyle(.gray)
 }
```

## See Also

### Creating store views that load products

init(ids: some Collection&lt;String>, prefersPromotionalIcon: Bool)

Creates a view to load and merchandise a collection of products from the App Store using product identifiers.

init(ids: some Collection&lt;String>, prefersPromotionalIcon: Bool, icon: (Product) -> Icon)

Creates a view to load a collection of products from the App Store using product identifiers, and merchandise them using a custom image.

init(ids: some Collection&lt;String>, icon: (Product, ProductIconPhase) -> Icon, placeholderIcon: () -> PlaceholderIcon)

Creates a view to load a collection of products from the App Store using product identifiers, and merchandise them using their promotional images and a custom placeholder icon.

