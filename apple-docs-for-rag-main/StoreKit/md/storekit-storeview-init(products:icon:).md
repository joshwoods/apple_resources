

- StoreKit
- StoreView
-  init(products:icon:) 

Initializer

# init(products:icon:)

Creates a view to merchandise a collection of products with promotional images.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
init(
    products: some Collection,
    @ViewBuilder icon: @escaping (Product, ProductIconPhase) -> Icon
) where PlaceholderIcon == EmptyView
```

## Parameters 

`products`  

The products to merchandise.

`icon`  

A closure that receives a Product and a ProductIconPhase as input. The ProductIconPhase indicates the state of the loading operation of the product’s promotional image. The closure returns the view to display for the given product and phase value.

## Discussion

The store view asynchronously loads and displays each product’s promotional image. Use the ProductIconPhase to monitor the current loading phase of the product’s promotional image, and provide an image for each phase. For more information about the loading phases, see ProductIconPhase.

## See Also

### Creating store views with preloaded products

init(products: some Collection&lt;Product>, prefersPromotionalIcon: Bool)

Creates a view to load and merchandise a collection of products from the App Store.

init(products: some Collection&lt;Product>, prefersPromotionalIcon: Bool, icon: (Product) -> Icon)

Creates a view to merchandise a collection of products using a custom icon.

