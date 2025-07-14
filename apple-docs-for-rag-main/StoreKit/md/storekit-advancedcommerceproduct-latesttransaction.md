

- StoreKit
- AdvancedCommerceProduct
-  latestTransaction 

Instance Property

# latestTransaction

The most recent transaction associated with the generic product ID, if it exists.

iOS 18.4+iPadOS 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
var latestTransaction: VerificationResult? { get async }
```

## Discussion

This value is `nil` if the customer hasn’t made any purchases associated with the generic product ID.

## See Also

### Getting transactions and entitlements

var allTransactions: Transaction.Transactions

All transactions associated with the generic product ID.

var currentEntitlements: Transaction.Transactions

The transactions that entitle the customer to Advanced Commerce Items purchased using the generic product ID.

