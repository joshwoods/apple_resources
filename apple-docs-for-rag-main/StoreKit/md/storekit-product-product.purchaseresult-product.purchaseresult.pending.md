

- StoreKit
- Product
- Product.PurchaseResult
-  Product.PurchaseResult.pending 

Case

# Product.PurchaseResult.pending

The purchase is pending, and requires action from the customer.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
case pending
```

## Discussion

If a pending purchase succeeds, StoreKit delivers the resulting Transaction in the transaction updates.

## See Also

### Getting the Purchase Results

case success(VerificationResult&lt;Transaction>)

The purchase succeeded and results in a transaction.

case userCancelled

The user canceled the purchase.

