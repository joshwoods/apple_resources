

- StoreKit
- Transaction
-  currentEntitlements 

Type Property

# currentEntitlements

A sequence of the latest transactions that entitle a customer to In-App Purchases and subscriptions.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var currentEntitlements: Transaction.Transactions { get }
```

## Mentioned in 

Supporting subscription offer codes in your app

Supporting win-back offers in your app

Supporting business model changes by using the app transaction

## Discussion

The current entitlements sequence emits the latest transaction for each product the customer has an entitlement to, specifically:

- A transaction for each non-consumable In-App Purchase

- The latest transaction for each auto-renewable subscription that has a Product.SubscriptionInfo.RenewalState state of subscribed or inGracePeriod

- The latest transaction for each non-renewing subscription, including finished ones

Products that the App Store has refunded or revoked don’t appear in the current entitlements. Consumable In-App Purchases also don’t appear in the current entitlements. To get transactions for unfinished consumables, use the unfinished or all sequences in Transaction.

The following example illustrates iterating through the current entitlements:

```
func refreshPurchasedProducts() async {
    // Iterate through the user's purchased products.
    for await verificationResult in Transaction.currentEntitlements {
        switch verificationResult {
        case .verified(let transaction):
            // Check the type of product for the transaction
            // and provide access to the content as appropriate.
            ...
        case .unverified(let unverifiedTransaction, let verificationError):
            // Handle unverified transactions based on your
            // business model.
            ...
        }
    }
}
```

## See Also

### Transaction history and entitlements

struct Transaction

Information that represents the customer’s purchase of a product in your app.

static var updates: Transaction.Transactions

The asynchronous sequence that emits a transaction when the system creates or updates transactions that occur outside the app or on other devices.

static var all: Transaction.Transactions

A sequence that emits all the customer’s transactions for your app.

