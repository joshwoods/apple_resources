

- StoreKit
-  SKPaymentQueue Deprecated

Class

# SKPaymentQueue

A queue of payment transactions for the App Store to process.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOS 9.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
class SKPaymentQueue
```

Deprecated

No longer supported

## Mentioned in 

Testing transaction observer code

Unlocking purchased content

Restoring purchased products

## Overview

The payment queue communicates with the App Store and presents a user interface so that the user can authorize payment. The contents of the queue are persistent between launches of your app.

To process a payment, first add at least one observer object (SKPaymentTransactionObserver) to the queue (see add(_:)). Then, add a payment object (SKPayment) for the item the user wants to purchase. Each time you add a payment object, the queue creates a transaction object (SKPaymentTransaction) to process that payment and enqueues it to be processed. After payment is fulfilled, the queue updates the transaction object and then calls any observer objects to provide them the updated transaction. Your observer should process the transaction and then remove it from the queue.

The exact mechanism you use to process a processed transaction depends on the design of your app and the product being purchased. Here are a few common examples:

- If the product is a feature already built into your app, your app enables the feature to process the transaction.

- If the product includes downloadable content provided by the App Store, your app retrieves the SKDownload objects from the transaction and ask the payment queue to download them. You provide the actual content files to be served by the App Store to App Store Connect when you create the product information.

- If the product represents downloadable content provided by your own server, your app might open a network connection to your server and download the content from there.

For more information on designing the payment processing portion of your app, see In-App Purchase Programming Guide.

## Topics

### Determining Whether the User Can Make Payments

class func canMakePayments() -> Bool

A method that indicates whether the person can make purchases.

### Determining Store Content

var storefront: SKStorefront?

The App Store storefront of the device.

### Getting the Queue

class func `default`() -> Self

Returns the default payment queue instance.

### Adding, Getting, and Removing Observers

func add(any SKPaymentTransactionObserver)

Adds an observer to the payment queue.

var transactionObservers: [any SKPaymentTransactionObserver]

An array of all active payment queue observers.

func remove(any SKPaymentTransactionObserver)

Removes an observer from the payment queue.

### Managing Transactions

var delegate: (any SKPaymentQueueDelegate)?

A delegate that provides information needed to complete transactions.

var transactions: [SKPaymentTransaction]

Returns an array of pending transactions.

func add(SKPayment)

Adds a payment request to the queue.

func finishTransaction(SKPaymentTransaction)

Notifies the App Store that the app finished processing the transaction.

### Restoring Purchases

func restoreCompletedTransactions()

Asks the payment queue to restore previously completed purchases.

func restoreCompletedTransactions(withApplicationUsername: String?)

Asks the payment queue to restore previously completed purchases, providing an opaque identifier for the user’s account.

### Showing Price Consent

func showPriceConsentIfNeeded()

Asks the system to display the price consent sheet if the user hasn’t yet responded to a subscription price increase.

### Redeeming Codes

func presentCodeRedemptionSheet()

Displays a sheet that enables customers to redeem subscription offer codes that you configure in App Store Connect.

### Downloading Content

func start([SKDownload])

Adds a set of downloads to the download list.

func cancel([SKDownload])

Removes a set of downloads from the download list.

func pause([SKDownload])

Pauses a set of downloads.

func resume([SKDownload])

Resumes a set of downloads.

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

### Essentials

Setting up the transaction observer for the payment queue

Enable your app to receive and handle transactions by adding an observer.

Offering, completing, and restoring in-app purchases

Fetch, display, purchase, validate, and finish transactions in your app.

protocol SKPaymentTransactionObserver

A set of methods that process transactions, unlock purchased functionality, and continue promoted In-App Purchases.

Deprecated

protocol SKPaymentQueueDelegate

The protocol that provides information needed to complete transactions.

Deprecated

class SKRequest

An abstract class that represents a request to the App Store.

Deprecated

