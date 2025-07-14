

- StoreKit
-  ProductViewStyle 

Protocol

# ProductViewStyle

A type that specifies the appearance and interaction of In-App Purchase products within the view hierarchy.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@MainActor @preconcurrency
protocol ProductViewStyle
```

## Overview

To configure the in-app purchase product style for a view hierarchy, use the productViewStyle(_:) modifier.

To create a custom style, declare a type that conforms to the `ProductViewStyle` protocol. Implement the makeBody(configuration:) method to return a view that composes the elements of the configuration that the system provides to your method. The following code example shows how to create a custom product view style:

```
struct CustomProductViewStyle: ProductViewStyle {
    func makeBody(configuration: Configuration) -> some View {
        switch configuration.state {
        // Add other cases here.
        case .success(let product):
            VStack(alignment: .center) {
                configuration.icon
                Text(product.displayName)
                Button(product.displayPrice) {}
            }
        }
    }
}

ProductView(id: "com.example.product")
    .productViewStyle(CustomProductViewStyle())
    // Add your code here.
```

## Topics

### Getting built-in product view styles

static var automatic: AutomaticProductViewStyle

static var compact: CompactProductViewStyle

An product view style suitable for layouts where less space is available, or for displaying more items in a small amount of space.

static var large: LargeProductViewStyle

A product view style suitable for layouts where the in-app purchase content is prominent.

static var regular: RegularProductViewStyle

A product view style that uses a standard, platform-appropriate layout.

### Creating custom product views

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view that represents the body of a product view.

**Required**

typealias Configuration

A type that represents the properties of a product view style.

associatedtype Body : View

A view that represents the body of a product view.

**Required**

### Supporting types

struct AutomaticProductViewStyle

struct CompactProductViewStyle

A style for a product view that’s suitable for layouts with less available space, or for displaying more items in a small amount of space.

struct RegularProductViewStyle

A style for a product view that uses a standard, platform-appropriate layout.

struct LargeProductViewStyle

A style for a product view that’s suitable for layouts where the in-app purchase content is prominent.

## Relationships

### Conforming Types

- AutomaticProductViewStyle
- CompactProductViewStyle
- LargeProductViewStyle
- RegularProductViewStyle

## See Also

### Styling product views

nonisolated func productViewStyle(_ style: some ProductViewStyle) -> some View 

Sets the style for In-App Purchase product views within a view.

nonisolated func productIconBorder() -> some View 

Adds a standard border to an in-app purchase product’s icon .

struct ProductViewStyleConfiguration

The properties of an In-App Purchase product for use by custom product view styles.

