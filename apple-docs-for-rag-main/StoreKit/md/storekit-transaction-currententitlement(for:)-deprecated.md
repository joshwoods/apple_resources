

- StoreKit
- Transaction
-  currentEntitlement(for:) Deprecated

Type Method

# currentEntitlement(for:)

Gets the latest transactions that entitle the customer to a specified product.

iOS 15.0–18.4DeprecatediPadOS 15.0–18.4DeprecatedmacOS 12.0–15.4DeprecatedtvOS 15.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 8.0–11.4Deprecated

``` source
static func currentEntitlement(for productID: String) async -> VerificationResult?
```

Deprecated

Use the currentEntitlements(for:) method instead.

## Parameters 

`productID`  

In-App Purchase product identifier.

## Return Value

A VerificationResult or `nil` if the customer has no current In-App Purchases.

## See Also

### Getting current entitlements

static var currentEntitlements: Transaction.Transactions

A sequence of the latest transactions that entitle a customer to In-App Purchases and subscriptions.

