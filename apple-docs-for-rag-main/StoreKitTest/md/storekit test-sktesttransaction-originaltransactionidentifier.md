

- StoreKit Test
- SKTestTransaction
-  originalTransactionIdentifier 

Instance Property

# originalTransactionIdentifier

The identifier of the original transaction.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var originalTransactionIdentifier: Int { get }
```

## Discussion

For subscription renewals, or if you restore a purchase, the originalTransactionIdentifier is the original transaction for that subscription or in-app purchase.

## See Also

### Identifying Transactions and Products

var identifier: Int

The identifier of the transaction in the testing environment.

var productIdentifier: String

An identifier that uniquely represents a product, which you provide in the StoreKit configuration file.

