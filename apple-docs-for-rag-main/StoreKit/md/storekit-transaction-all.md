

- StoreKit
- Transaction
-  all 

Type Property

# all

A sequence that emits all the customer’s transactions for your app.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var all: Transaction.Transactions { get }
```

## Mentioned in 

Supporting win-back offers in your app

Supporting subscription offer codes in your app

## Discussion

This sequence returns the customer’s transaction history current to the moment you access it. The sequence emits a finite number of transactions. If the App Store processes additional transactions for the customer while you’re accessing this sequence, they appear in the transaction listener updates.

The transaction history includes the following in-app purchases:

- Unfinished consumables

- Finished consumables that are refunded or revoked

- Non-consumables

- Auto-renewable subscriptions, including all renewals

- Auto-renewable subscriptions and non-consumables that the customer gets through Family Sharing

By default, when the SKIncludeConsumableInAppPurchaseHistory property list key is `false`, the transaction information excludes finished consumables (unless refunded or revoked).

To get all possible transactions, including all finished consumables, set the SKIncludeConsumableInAppPurchaseHistory property list key to `true`.

## See Also

### Transaction history and entitlements

struct Transaction

Information that represents the customer’s purchase of a product in your app.

static var updates: Transaction.Transactions

The asynchronous sequence that emits a transaction when the system creates or updates transactions that occur outside the app or on other devices.

static var currentEntitlements: Transaction.Transactions

A sequence of the latest transactions that entitle a customer to In-App Purchases and subscriptions.

