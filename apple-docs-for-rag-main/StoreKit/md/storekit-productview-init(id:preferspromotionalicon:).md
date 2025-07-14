

- StoreKit
- ProductView
-  init(id:prefersPromotionalIcon:) 

Initializer

# init(id:prefersPromotionalIcon:)

Creates a view to load and merchandise an individual product from the App Store.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
init(
    id productID: Product.ID,
    prefersPromotionalIcon: Bool = false
) where Icon == EmptyView, PlaceholderIcon == EmptyView
```

## Parameters 

`productID`  

The product identifier to load from the App Store.

`prefersPromotionalIcon`  

A Boolean value that indicates whether to use the promotional image from the App Store, if it’s available. If this parameter is `false`, the system ignores any promotional images.

## Discussion

By default, the view doesn’t show an icon. If you set the `prefersPromotionalIcon` parameter to `true`, the view displays a placeholder icon while loading, and replaces the placeholder with the promotional image for the product.

Tip

To gain more control over the image that decorates this view, use the init(id:icon:placeholderIcon:) initializer. It receives a ProductIconPhase, which enables you to supply an image for each phase of the image-loading process.

## See Also

### Creating product views that load products

init(id: Product.ID, prefersPromotionalIcon: Bool, icon: () -> Icon)

Creates a view to load an individual product from the App Store and merchandise it using a custom icon.

init(id: Product.ID, prefersPromotionalIcon: Bool, icon: () -> Icon, placeholderIcon: () -> PlaceholderIcon)

Creates a view to load an individual product from the App Store and merchandise it using an image and a custom placeholder icon.

init(id: Product.ID, icon: (ProductIconPhase) -> Icon, placeholderIcon: () -> PlaceholderIcon)

Creates a view to load an individual product from the App Store, and merchandise it using its promotional image and a custom placeholder icon.

