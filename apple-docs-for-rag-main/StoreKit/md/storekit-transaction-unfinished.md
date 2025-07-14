

- StoreKit
- Transaction
-  unfinished 

Type Property

# unfinished

A sequence that emits unfinished transactions for the customer.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var unfinished: Transaction.Transactions { get }
```

## Discussion

A transaction is unfinished until you call finish(). Use the unfinished sequence to find the transactions your app needs to process to deliver purchased content or enable service.

## See Also

### Getting transaction history

static func latest(for: String) async -> VerificationResult&lt;Transaction>?

Gets the customer’s most recent transaction for an In-App Purchase.

static var all: Transaction.Transactions

A sequence that emits all the customer’s transactions for your app.

SKIncludeConsumableInAppPurchaseHistory

A Boolean value that determines whether StoreKit includes finished consumable In-App Purchases in transaction information.

