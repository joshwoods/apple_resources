

- StoreKit
- ProductView
-  init(\_:prefersPromotionalIcon:icon:) 

Initializer

# init(\_:prefersPromotionalIcon:icon:)

Creates a view to merchandise an individual product using a custom icon.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
init(
    _ product: Product,
    prefersPromotionalIcon: Bool = false,
    @ViewBuilder icon: () -> Icon
) where PlaceholderIcon == EmptyView
```

## Parameters 

`product`  

The product to merchandise.

`prefersPromotionalIcon`  

A Boolean value that indicates whether to use the promotional image from the App Store, if it’s available. If this value is `true` and a promotional image for the product is available, the view displays it instead of the view you provide in the `icon` parameter.

`icon`  

A closure that returns the image to use for decorating the in-app purchase product.

## Discussion

If `prefersPromotionalIcon` is `true` and the product has a promotional image, the view displays the promotional image instead of the view you provide in `icon`.

The following example shows how to create a product view using a custom icon:

```
ProductView(product) {
    Image(systemName: "star.fill")
        .foregroundStyle(.yellow)
}
```

Tip

To gain more control over the image that decorates this view, use the init(_:icon:) initializer. It receives a ProductIconPhase, which enables you to supply an image for each phase of the image-loading process.

## See Also

### Creating product views with preloaded products

init(Product, prefersPromotionalIcon: Bool)

Creates a view to merchandise an individual product.

init(Product, icon: (ProductIconPhase) -> Icon)

Creates a view to display a product that the system already loaded from the App Store, and merchandise it using its promotional image.

