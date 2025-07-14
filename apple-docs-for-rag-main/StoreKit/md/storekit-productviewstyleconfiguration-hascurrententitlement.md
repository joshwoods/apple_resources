

- StoreKit
- ProductViewStyleConfiguration
-  hasCurrentEntitlement 

Instance Property

# hasCurrentEntitlement

A Boolean value that indicates whether an in-app purchase transaction exists for the product.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
let hasCurrentEntitlement: Bool
```

## Discussion

Use the hasCurrentEntitlement property to determine whether a purchase may succeed, for a porduct that people can purchase only once. For example, if hasCurrentEntitlement is false, you may choose not to display a purchase button for the product, because the person has already purchased it.

Important

Don’t use this value to determine whether to enable access to the product; check the in-app purchase transaction information instead (Transaction).

## See Also

### Getting a product’s information

var product: Product?

The in-app purchase product to merchandise.

let state: Product.TaskState

The product task state that indicates the product’s loading phase.

