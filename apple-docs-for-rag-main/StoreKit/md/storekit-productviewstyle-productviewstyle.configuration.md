

- StoreKit
- ProductViewStyle
-  ProductViewStyle.Configuration 

Type Alias

# ProductViewStyle.Configuration

A type that represents the properties of a product view style.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
typealias Configuration = ProductViewStyleConfiguration
```

## See Also

### Creating custom product views

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view that represents the body of a product view.

**Required**

associatedtype Body : View

A view that represents the body of a product view.

**Required**

