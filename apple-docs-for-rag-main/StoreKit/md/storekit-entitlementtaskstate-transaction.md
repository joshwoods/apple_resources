

- StoreKit
- EntitlementTaskState
-  transaction 

Instance Property

# transaction

The transaction value if the task is successful.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var transaction: VerificationResult? { get }
```

Available when `Value` is `VerificationResult?`.

## Discussion

Use transaction as a convenience to access the transaction value in code that doesn’t depend on the reason a transaction isn’t available. The value is `nil` while the transaction is loading, if it fails to load for any reason, or if the customer isn’t entitled to the product.

## See Also

### Getting the transaction with the entitlement

var value: Value?

The entitlement value if the task is successful.

