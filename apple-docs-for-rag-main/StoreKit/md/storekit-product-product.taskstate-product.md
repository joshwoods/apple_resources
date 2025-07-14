

- StoreKit
- Product
- Product.TaskState
-  product 

Instance Property

# product

The product value if the task was successful.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var product: Product? { get }
```

## Discussion

Use this as a convenience to access the product value in code that doesn’t depend on the reason the product can’t be accessed. The value is `nil` while the product is loading, or if the product can’t be accessed for any reason.

