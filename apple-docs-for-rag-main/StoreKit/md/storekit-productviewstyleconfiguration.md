

- StoreKit
-  ProductViewStyleConfiguration 

Structure

# ProductViewStyleConfiguration

The properties of an In-App Purchase product for use by custom product view styles.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct ProductViewStyleConfiguration
```

## Overview

Use the `ProductViewStyleConfiguration` to create a custom ProductViewStyle.

## Topics

### Getting a product’s information

var product: Product?

The in-app purchase product to merchandise.

let state: Product.TaskState

The product task state that indicates the product’s loading phase.

let hasCurrentEntitlement: Bool

A Boolean value that indicates whether an in-app purchase transaction exists for the product.

### Getting a product view’s icon

let icon: ProductViewStyleConfiguration.Icon

A decorative view for merchandising the product.

struct Icon

A type-erased icon of an in-app purchase product.

### Getting a product’s description visibility

let descriptionVisibility: Visibility

The visibility of product descriptions.

### Initiating a purchase

func purchase()

Initiates a purchase action for the product.

## See Also

### Styling product views

nonisolated func productViewStyle(_ style: some ProductViewStyle) -> some View 

Sets the style for In-App Purchase product views within a view.

nonisolated func productIconBorder() -> some View 

Adds a standard border to an in-app purchase product’s icon .

protocol ProductViewStyle

A type that specifies the appearance and interaction of In-App Purchase products within the view hierarchy.

