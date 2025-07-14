

- StoreKit
- ProductView
-  init(\_:icon:) 

Initializer

# init(\_:icon:)

Creates a view to display a product that the system already loaded from the App Store, and merchandise it using its promotional image.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
init(
    _ product: Product,
    @ViewBuilder icon: @escaping (ProductIconPhase) -> Icon
) where PlaceholderIcon == EmptyView
```

## Parameters 

`product`  

The product to merchandise.

`icon`  

A closure that receives a ProductIconPhase as an input, which indicates the state of the loading operation of the product’s promoted image, and returns the view to display for the specified phase.

## Discussion

The product view asynchronously loads and displays the product’s promotional image.

The ProductIconPhase value indicates whether the promotional image is loading, unavailable, or whether it succeeded or failed to load. Use the ProductIconPhase to monitor current loading phase, and to decide the image to return in the `icon` closure.

## See Also

### Creating product views with preloaded products

init(Product, prefersPromotionalIcon: Bool, icon: () -> Icon)

Creates a view to merchandise an individual product using a custom icon.

init(Product, prefersPromotionalIcon: Bool)

Creates a view to merchandise an individual product.

