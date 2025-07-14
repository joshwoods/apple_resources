

- StoreKit
- ProductView
-  init(id:prefersPromotionalIcon:icon:) 

Initializer

# init(id:prefersPromotionalIcon:icon:)

Creates a view to load an individual product from the App Store and merchandise it using a custom icon.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
init(
    id productID: Product.ID,
    prefersPromotionalIcon: Bool = false,
    @ViewBuilder icon: () -> Icon
) where PlaceholderIcon == AutomaticProductPlaceholderIcon
```

## Parameters 

`productID`  

The product identifier to load from the App Store.

`prefersPromotionalIcon`  

A Boolean value that indicates whether to use the promotional image from the App Store, if it’s available. If this value is `true` and a promotional image for the product is available, the view displays it instead of the view you provide in the `icon` parameter.

`icon`  

A closure that returns the image the view displays when the system finishes loading the product from the App Store.

## Discussion

The product view displays a placeholder icon until the system finishes loading the product. After the product loads, the system uses the view you provide in the `icon` parameter, by default. If `prefersPromotionalIcon` is `true` and the product has a promotional image, the view displays the promotional image as its icon instead of the provided view.

Tip

To gain more control over the image that decorates this view, use the init(id:icon:placeholderIcon:) initializer. It receives a ProductIconPhase, which enables you to supply an image for each phase of the image-loading process.

## See Also

### Creating product views that load products

init(id: Product.ID, prefersPromotionalIcon: Bool)

Creates a view to load and merchandise an individual product from the App Store.

init(id: Product.ID, prefersPromotionalIcon: Bool, icon: () -> Icon, placeholderIcon: () -> PlaceholderIcon)

Creates a view to load an individual product from the App Store and merchandise it using an image and a custom placeholder icon.

init(id: Product.ID, icon: (ProductIconPhase) -> Icon, placeholderIcon: () -> PlaceholderIcon)

Creates a view to load an individual product from the App Store, and merchandise it using its promotional image and a custom placeholder icon.

