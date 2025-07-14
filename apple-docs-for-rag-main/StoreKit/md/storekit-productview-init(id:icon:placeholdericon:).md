

- StoreKit
- ProductView
-  init(id:icon:placeholderIcon:) 

Initializer

# init(id:icon:placeholderIcon:)

Creates a view to load an individual product from the App Store, and merchandise it using its promotional image and a custom placeholder icon.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
init(
    id productID: Product.ID,
    @ViewBuilder icon: @escaping (ProductIconPhase) -> Icon,
    @ViewBuilder placeholderIcon: () -> PlaceholderIcon
)
```

## Parameters 

`productID`  

The product identifier to load from the App Store.

`icon`  

A closure that receives a ProductIconPhase as an input, which indicates the state of the loading operation of the product’s promotional image, and returns the view to display for the specified phase.

`placeholderIcon`  

A closure that returns an icon to display until the system finishes loading the product from the App Store.

## Discussion

The product view shows the `placeholderIcon` until the system finishes loading the product. After the product finishes loading, the view asynchronously loads and displays the product’s promotional image. Use the ProductIconPhase to monitor the current loading state of the product’s promotional image.

If the product is unavailable, the view displays the `placeholderIcon` as a fallback.

The ProductIconPhase value indicates whether the promotional image is loading, unavailable, or whether it succeeded or failed to load. Use the phase to decide what to draw. While the image’s loading operation is in the ProductIconPhase.loading phase, consider displaying the same view that you provide in the `placeholderIcon` closure. For more information, see ProductIconPhase.

## See Also

### Creating product views that load products

init(id: Product.ID, prefersPromotionalIcon: Bool)

Creates a view to load and merchandise an individual product from the App Store.

init(id: Product.ID, prefersPromotionalIcon: Bool, icon: () -> Icon)

Creates a view to load an individual product from the App Store and merchandise it using a custom icon.

init(id: Product.ID, prefersPromotionalIcon: Bool, icon: () -> Icon, placeholderIcon: () -> PlaceholderIcon)

Creates a view to load an individual product from the App Store and merchandise it using an image and a custom placeholder icon.

