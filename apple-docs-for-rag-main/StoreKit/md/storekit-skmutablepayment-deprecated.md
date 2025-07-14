

- StoreKit
-  SKMutablePayment Deprecated

Class

# SKMutablePayment

A mutable request to the App Store to process payment for additional functionality that your app offers.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
class SKMutablePayment
```

Deprecated

Use Product.purchase(confirmIn:options:)

## Mentioned in 

Implementing promotional offers in your app

## Overview

A mutable payment object identifies a product and the quantity of that item the user would like to purchase.

When a mutable payment is added to the payment queue, the payment queue copies the contents into an immutable request before queueing the request. Your app can safely change the contents of the mutable payment object.

## Topics

### Getting and Setting Attributes

var productIdentifier: String

A string that identifies a product that can be purchased from within your app.

var quantity: Int

The number of items the user wants to purchase.

var requestData: Data?

Reserved for future use.

var applicationUsername: String?

A string that associates the transaction with a user account on your service.

### Simulating Buy for Testing

var simulatesAskToBuyInSandbox: Bool

A Boolean value that produces an “ask to buy” flow for this payment in the sandbox.

### Getting and Setting Discount Details

var paymentDiscount: SKPaymentDiscount?

The details of the discount offer to apply to the payment.

## Relationships

### Inherits From

- SKPayment

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSMutableCopying
- NSObjectProtocol

## See Also

### Purchases

Requesting a payment from the App Store

Submit a payment request to the App Store when a customer selects a product to buy.

Processing a transaction

Register a transaction queue observer to get and handle transaction updates from the App Store.

class SKPayment

A request to the App Store to process payment for additional functionality that your app offers.

Deprecated

class SKPaymentTransaction

An object in the payment queue.

Deprecated

