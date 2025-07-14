

- StoreKit
- ProductView
-  init(\_:) 

Initializer

# init(\_:)

Creates a view to merchandise an individual product using a configuration for product view style.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
init(_ configuration: ProductViewStyleConfiguration) where Icon == ProductViewStyleConfiguration.Icon, PlaceholderIcon == ProductViewStyleConfiguration.Icon
```

## Parameters 

`configuration`  

A configuration for a product view style.

## Discussion

Use this initializer within the makeBody(configuration:) method of a ProductViewStyle to create an instance of the product view you want to style. This is useful for custom product view styles that modify the current style, rather than implementing a new style.

The following code example shows how to create and use custom styles by composing standard styles:

```
struct SpinnerWhenLoadingStyle: ProductViewStyle {
    public func makeBody(configuration: Configuration) -> some View {
        switch configuration.state {
        case .loading:
            ProgressView()
                .progressView(.circular)
        default:
            ProductView(configuration)
        }
    }
}
// Use the following elsewhere in the code.
ProductView(id: "com.example.product")
    .productViewStyle(SpinnerWhenLoadingStyle())
```

