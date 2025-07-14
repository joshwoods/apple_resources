

- StoreKit
-  SKRequest Deprecated

Class

# SKRequest

An abstract class that represents a request to the App Store.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
class SKRequest
```

Deprecated

No longer supported

## Overview

To make a request, initialize a subclass of SKRequest—such as SKProductsRequest or SKReceiptRefreshRequest—set the delegate property, and call the start() method.

## Topics

### Controlling the Request

func start()

Sends the request to the Apple App Store.

func cancel()

Cancels a previously started request.

### Accessing the Delegate

var delegate: (any SKRequestDelegate)?

The delegate of the request object.

protocol SKRequestDelegate

Common methods that are implemented by delegates for any subclass of the `SKRequest` abstract class.

## Relationships

### Inherits From

- NSObject

### Inherited By

- SKProductsRequest
- SKReceiptRefreshRequest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
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

protocol SKPaymentQueueDelegate

The protocol that provides information needed to complete transactions.

Deprecated

