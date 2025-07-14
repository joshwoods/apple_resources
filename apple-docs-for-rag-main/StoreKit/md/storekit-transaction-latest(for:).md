

- StoreKit
- Transaction
-  latest(for:) 

Type Method

# latest(for:)

Gets the customer’s most recent transaction for an In-App Purchase.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func latest(for productID: String) async -> VerificationResult?
```

## Parameters 

`productID`  

The product identifier that the method uses to look up the most recent transaction.

## Return Value

A VerificationResult with a single Transaction, or `nil` if the customer hasn’t purchased the product.

## Discussion

Call this method for any type of In-App Purchase. The following code example illustrates requesting the most recent transaction to determine whether the customer purchased the product indicated by the string `productIdentifier`:

```
guard let verificationResult = await Transaction.latest(for: productIdentifier) else {    
    // The customer hasn't purchased this product.
    return
}

switch verificationResult {
case .verified(let transaction):
    // Check the transaction and give the customer access to purchased 
    // content as appropriate.
    ...
case .unverified(let transaction, let verificationError):
    // Handle unverified transactions based 
    // on your business model.
    ...
}
```

By default, when the SKIncludeConsumableInAppPurchaseHistory property list key is `false`, this method excludes finished consumable in-app purchases unless they are refunded or revoked.

If you set the SKIncludeConsumableInAppPurchaseHistory property list key to `true`, this method returns all transactions, including consumable In-App Purchases that your app marked as finished (finish()).

## See Also

### Getting transaction history

static var all: Transaction.Transactions

A sequence that emits all the customer’s transactions for your app.

static var unfinished: Transaction.Transactions

A sequence that emits unfinished transactions for the customer.

SKIncludeConsumableInAppPurchaseHistory

A Boolean value that determines whether StoreKit includes finished consumable In-App Purchases in transaction information.

