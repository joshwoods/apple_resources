

- StoreKit
- ProductViewStyle
-  makeBody(configuration:) 

Instance Method

# makeBody(configuration:)

Creates a view that represents the body of a product view.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@ViewBuilder @MainActor @preconcurrency
func makeBody(configuration: Self.Configuration) -> Self.Body
```

**Required**

## Parameters 

`configuration`  

The properties of a product view style.

## See Also

### Creating custom product views

typealias Configuration

A type that represents the properties of a product view style.

associatedtype Body : View

A view that represents the body of a product view.

**Required**

