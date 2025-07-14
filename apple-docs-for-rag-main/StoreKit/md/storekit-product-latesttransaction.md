

- StoreKit
- Product
-  latestTransaction 

Instance Property

# latestTransaction

The most recent transaction for the product.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var latestTransaction: VerificationResult? { get async }
```

## Discussion

This value is `nil` if the customer has never purchased this product. The following code example illustrates requesting the most recent transaction for a product to determine whether the customer has purchased the product:

```
guard let resultingTransaction = await product.latestTransaction else {
    // The customer hasn't purchased this product.
    return
}
guard case .verified(let transaction) = resultingTransaction else {
    // Ignore unverified transactions.
    return
}
// Update your app based on the details from the most recent transaction.
```

By default, when the SKIncludeConsumableInAppPurchaseHistory property list key is `false`, this value excludes finished consumable in-app purchases unless they are refunded or revoked.

If you set the SKIncludeConsumableInAppPurchaseHistory property list key to `true`, this value returns all transactions, including consumable in-app purchases that your app marked as finished (finish()).

