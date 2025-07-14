

- StoreKit
-  SKPaymentTransaction Deprecated

Class

# SKPaymentTransaction

An object in the payment queue.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
class SKPaymentTransaction
```

Deprecated

Use PurchaseResult from Product.purchase(confirmIn:options:)

## Mentioned in 

Restoring purchased products

Implementing promotional offers in your app

## Overview

A payment transaction is created whenever a payment is added to the payment queue. The system delivers transactions to your app when the App Store finishes processing the payment. Completed transactions provide a receipt and transaction identifier that your app can use to save a permanent record of the processed payment.

## Topics

### Getting Transaction Information

var payment: SKPayment

The payment for the transaction.

var transactionIdentifier: String?

A string that uniquely identifies a successful payment transaction.

var transactionDate: Date?

The date the transaction was added to the App Store’s payment queue.

var original: SKPaymentTransaction?

The transaction that was restored by the App Store.

var error: (any Error)?

An object describing the error that occurred while processing the transaction.

var transactionReceipt: Data?

A signed receipt that records all information about a successful payment transaction.

### Getting Downloads

var downloads: [SKDownload]

An array of download objects representing the downloadable content associated with the transaction.

### Getting Transaction State

var transactionState: SKPaymentTransactionState

The current state of the transaction.

enum SKPaymentTransactionState

Values representing the state of a transaction.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Purchases

Requesting a payment from the App Store

Submit a payment request to the App Store when a customer selects a product to buy.

Processing a transaction

Register a transaction queue observer to get and handle transaction updates from the App Store.

class SKPayment

A request to the App Store to process payment for additional functionality that your app offers.

Deprecated

class SKMutablePayment

A mutable request to the App Store to process payment for additional functionality that your app offers.

Deprecated

