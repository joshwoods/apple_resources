

- StoreKit
-  ProductView 

Structure

# ProductView

A view that merchandises an individual In-App Purchase product.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@MainActor @preconcurrency
struct ProductView where Icon : View, PlaceholderIcon : View
```

## Overview

A `ProductView` shows information about an in-app purchase product, including its localized name, description, and price, and displays a purchase button.

You create a product view by providing a product identifier to load from the App Store, or a Product value you previously loaded. If you provide a product identifier, the view loads the product’s information from the App Store automatically, and updates the view when the product is available.

You can customize the view by providing a view to use as an icon, or image, for the in-app purchase product. If you provide a product identifier, you can optionally provide a placeholder icon for the system to use instead of the automatic placeholder icon. If you set up promoted images for your products in App Store Connect, you can choose to use those images as the icon.

You can customize the product view’s appearance using the standard styles, including the CompactProductViewStyle, RegularProductViewStyle, and LargeProductViewStyle styles. Apply the style using the productViewStyle(_:) view modifier.

You can also create your own custom styles by creating styles that conform to the ProductViewStyle protocol.

## Topics

### Creating product views that load products

init(id: Product.ID, prefersPromotionalIcon: Bool)

Creates a view to load and merchandise an individual product from the App Store.

init(id: Product.ID, prefersPromotionalIcon: Bool, icon: () -> Icon)

Creates a view to load an individual product from the App Store and merchandise it using a custom icon.

init(id: Product.ID, prefersPromotionalIcon: Bool, icon: () -> Icon, placeholderIcon: () -> PlaceholderIcon)

Creates a view to load an individual product from the App Store and merchandise it using an image and a custom placeholder icon.

init(id: Product.ID, icon: (ProductIconPhase) -> Icon, placeholderIcon: () -> PlaceholderIcon)

Creates a view to load an individual product from the App Store, and merchandise it using its promotional image and a custom placeholder icon.

### Creating product views with preloaded products

init(Product, prefersPromotionalIcon: Bool, icon: () -> Icon)

Creates a view to merchandise an individual product using a custom icon.

init(Product, prefersPromotionalIcon: Bool)

Creates a view to merchandise an individual product.

init(Product, icon: (ProductIconPhase) -> Icon)

Creates a view to display a product that the system already loaded from the App Store, and merchandise it using its promotional image.

### Creating product views with a configuration

init(ProductViewStyleConfiguration)

Creates a view to merchandise an individual product using a configuration for product view style.

### Loading promotional images

enum ProductIconPhase

The current phase of the asynchronous loading operation of a product’s promotional image.

### Supporting types

struct AutomaticProductPlaceholderIcon

A view that represents the default placeholder icon for an in-app store product.

## Relationships

### Conforms To

- Sendable
- View

## See Also

### Merchandising In-App Purchases and subscriptions

struct StoreView

A view that merchandises a collection of In-App Purchase products.

struct SubscriptionStoreView

A view that merchandises a collection of auto-renewable subscription options that belong to the same subscription group.

Backyard Birds: Building an app with SwiftData and widgets

Create an app with persistent data, interactive widgets, and an all new in-app purchase experience.

