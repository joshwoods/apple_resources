

- StoreKit
- Product
- Product.CollectionTaskState
-  products 

Instance Property

# products

An array of available products if the task was successful.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var products: [Product]? { get }
```

## Discussion

Use this as a convenience to access the products in code that doesn’t depend on the reason the reason a product can’t be accessed. The value is `nil` while the task is loading, or if the task fails.

