

- StoreKit
-  SKPaymentTransactionObserver Deprecated

Protocol

# SKPaymentTransactionObserver

A set of methods that process transactions, unlock purchased functionality, and continue promoted In-App Purchases.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOS 9.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
protocol SKPaymentTransactionObserver : NSObjectProtocol
```

Deprecated

Use StoreKit 2 Transaction APIs

## Mentioned in 

Testing In-App Purchases in Xcode

Promoting In-App Purchases

Setting up the transaction observer for the payment queue

Processing a transaction

Testing transaction observer code

## Overview

Observers of SKPaymentQueue objects implement the methods of this protocol.

The system calls an observer when the queue updates or removes transactions. An observer needs to process all successful transactions, unlock the functionality the user purchases, and then finish the transaction by calling the payment queue’s finishTransaction(_:) method.

## Topics

### Handling transactions

func paymentQueue(SKPaymentQueue, updatedTransactions: [SKPaymentTransaction])

Tells an observer that one or more transactions have been updated.

**Required**

func paymentQueue(SKPaymentQueue, removedTransactions: [SKPaymentTransaction])

Tells an observer that one or more transactions have been removed from the queue.

### Restoring transactions

func paymentQueue(SKPaymentQueue, restoreCompletedTransactionsFailedWithError: any Error)

Tells the observer that an error occurred while restoring transactions.

func paymentQueueRestoreCompletedTransactionsFinished(SKPaymentQueue)

Tells the observer that the payment queue has finished sending restored transactions.

### Handling promoted in-app purchases

Promoting In-App Purchases

Show promoted In-App Purchases on your product page and handle purchases that customers initiate on the App Store.

func paymentQueue(SKPaymentQueue, shouldAddStorePayment: SKPayment, for: SKProduct) -> Bool

Tells the observer when a user initiates an in-app purchase from the App Store.

### Revoking entitlements

func paymentQueue(SKPaymentQueue, didRevokeEntitlementsForProductIdentifiers: [String])

Tells an observer that the customer is no longer entitled to one or more Family Sharing purchases.

### Changing the storefront

func paymentQueueDidChangeStorefront(SKPaymentQueue)

Tells the observer that the storefront for the payment queue has changed.

### Handling download actions

func paymentQueue(SKPaymentQueue, updatedDownloads: [SKDownload])

Tells the observer that the payment queue has updated one or more download objects.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Essentials

Setting up the transaction observer for the payment queue

Enable your app to receive and handle transactions by adding an observer.

Offering, completing, and restoring in-app purchases

Fetch, display, purchase, validate, and finish transactions in your app.

class SKPaymentQueue

A queue of payment transactions for the App Store to process.

Deprecated

protocol SKPaymentQueueDelegate

The protocol that provides information needed to complete transactions.

Deprecated

class SKRequest

An abstract class that represents a request to the App Store.

Deprecated

