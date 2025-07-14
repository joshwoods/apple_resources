

- StoreKit Test
-  SKTestTransaction 

Class

# SKTestTransaction

A transaction that occurs in the testing environment.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
class SKTestTransaction
```

## Overview

The test transaction represents the test environment’s knowledge of the transaction, including its identifier and the transaction’s state. It represents all the transaction-related configurations you control manually in Xcode for interrupted purchases, Ask to Buy scenarios, and changes to a subscription’s auto-renew state.

The test environment creates an `SKTestTransaction` instance each time your test code calls any method of SKTestSession that affects in-app purchases.

## Topics

### Identifying Transactions and Products

var identifier: Int

The identifier of the transaction in the testing environment.

var originalTransactionIdentifier: Int

The identifier of the original transaction.

var productIdentifier: String

An identifier that uniquely represents a product, which you provide in the StoreKit configuration file.

### Getting Payment Transaction States

var state: SKPaymentTransactionState

The state of the transaction in the test environment.

### Getting Dates

var purchaseDate: Date

The date of purchase for the transaction.

var cancelDate: Date?

The date when the system refunded the transaction.

var expirationDate: Date?

The date a subscription expires.

### Getting Test Environment States

var autoRenewingEnabled: Bool

A Boolean value that indicates whether automatic renewal is enabled for the subscription.

var hasPurchaseIssue: Bool

A Boolean value that indicates whether you resolve this transaction using the test framework functions.

var isPendingPriceIncreaseConsent: Bool

A Boolean value that indicates whether the auto-renewable subscription has a price increase that’s awaiting user consent in the test environment.

var pendingAskToBuyConfirmation: Bool

A Boolean value that indicates whether the transaction is awaiting an Ask to Buy confirmation.

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

### StoreKit transaction testing

Setting up StoreKit Testing in Xcode

Prepare your test environment to test in-app purchases with data you configure locally.

class SKTestSession

The controls and environment configuration you use to test StoreKit transactions in Xcode.

