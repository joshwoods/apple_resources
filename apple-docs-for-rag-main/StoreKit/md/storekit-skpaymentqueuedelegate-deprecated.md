

- StoreKit
-  SKPaymentQueueDelegate Deprecated

Protocol

# SKPaymentQueueDelegate

The protocol that provides information needed to complete transactions.

iOS 13.0–18.0DeprecatediPadOS 13.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.15–15.0DeprecatedtvOS 13.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
protocol SKPaymentQueueDelegate : NSObjectProtocol
```

Deprecated

No longer supported

## Overview

This protocol includes a method that lets your app determine whether to continue a transaction if the customer’s App Store storefront changes.

## Topics

### Continuing transactions

func paymentQueue(SKPaymentQueue, shouldContinue: SKPaymentTransaction, in: SKStorefront) -> Bool

Asks the delegate whether to continue the transaction if the device’s App Store storefront changes during a transaction.

### Showing price consent

func paymentQueueShouldShowPriceConsent(SKPaymentQueue) -> Bool

Asks the delegate whether to immediately display a price consent sheet.

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

protocol SKPaymentTransactionObserver

A set of methods that process transactions, unlock purchased functionality, and continue promoted In-App Purchases.

Deprecated

class SKRequest

An abstract class that represents a request to the App Store.

Deprecated

