

- StoreKit
- StoreView
-  init(products:prefersPromotionalIcon:) 

Initializer

# init(products:prefersPromotionalIcon:)

Creates a view to load and merchandise a collection of products from the App Store.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
init(
    products: some Collection,
    prefersPromotionalIcon: Bool = false
) where Icon == EmptyView, PlaceholderIcon == EmptyView
```

## Parameters 

`products`  

The products to merchandise.

`prefersPromotionalIcon`  

A Boolean value that indicates whether to use promotional images from the App Store, if they’re available. If this parameter is `false`, the system ignores promotional images.

## Discussion

By default, the store view doesn’t show promotional images. If you set `prefersPromotionalIcon` to `true`, the store view uses each product’s promotional image as its icon.

## See Also

### Creating store views with preloaded products

init(products: some Collection&lt;Product>, prefersPromotionalIcon: Bool, icon: (Product) -> Icon)

Creates a view to merchandise a collection of products using a custom icon.

init(products: some Collection&lt;Product>, icon: (Product, ProductIconPhase) -> Icon)

Creates a view to merchandise a collection of products with promotional images.

