

- StoreKit Test
- SKTestTransaction
-  identifier 

Instance Property

# identifier

The identifier of the transaction in the testing environment.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var identifier: Int { get }
```

## Discussion

To get a list of all the transactions available in the testing environment, see allTransactions().

Use this identifier if you want to perform actions on the transaction in the testing environment, such as:

- approveAskToBuyTransaction(identifier:)

- consentToPriceIncreaseForTransaction(identifier:)

- declineAskToBuyTransaction(identifier:)

- declinePriceIncreaseForTransaction(identifier:)

- deleteTransaction(identifier:)

- disableAutoRenewForTransaction(identifier:)

- enableAutoRenewForTransaction(identifier:)

- refundTransaction(identifier:)

- requestPriceIncreaseConsentForTransaction(identifier:)

- resolveIssueForTransaction(identifier:)

## See Also

### Identifying Transactions and Products

var originalTransactionIdentifier: Int

The identifier of the original transaction.

var productIdentifier: String

An identifier that uniquely represents a product, which you provide in the StoreKit configuration file.

