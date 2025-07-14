

- StoreKit
- AdvancedCommerceProduct
-  init(id:) 

Initializer

# init(id:)

Creates an Advanced Commerce product.

iOS 18.4+iPadOS 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
init(id: AdvancedCommerceProduct.ID) async throws
```

## Discussion

If given the product ID of an in-app purchase that doesn’t have access to Advanced Commerce API, this initializer throws StoreKitError.unsupported.

