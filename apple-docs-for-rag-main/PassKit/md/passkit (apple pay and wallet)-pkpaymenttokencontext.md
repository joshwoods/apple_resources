

- PassKit (Apple Pay and Wallet)
-  PKPaymentTokenContext 

Class

# PKPaymentTokenContext

A class that defines the context for a single payment token in a payment request for multimerchant payments.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class PKPaymentTokenContext
```

## Overview

Important

You must set the multiTokenContexts property on the PKPaymentRequest object to use this class to request multimerchant payments.

Use PKPaymentTokenContext to authorize a payment amount for each payment token in a multimerchant payment request. To enable multiple merchants for a transaction, use one PKPaymentTokenContext object for each merchant.

You can optionally associate each payment token with the merchant’s top-level domain.

## Topics

### Creating a payment token context

init(merchantIdentifier: String, externalIdentifier: String, merchantName: String, merchantDomain: String?, amount: NSDecimalNumber)

Create a payment token context for a single merchant.

### Specifying the merchant

var merchantIdentifier: String

The Apply Pay merchant identifier.

var merchantDomain: String?

The merchant’s top-level domain that the Apple Pay server associates with the payment token.

var merchantName: String

The merchant’s display name that the Apple Pay server associates with the payment token.

var externalIdentifier: String

An external identifier for the merchant.

### Indicating a payment amount

var amount: NSDecimalNumber

The amount to authorize for the payment token.

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

## See Also

### Payment requests

class PKPaymentRequest

An object that represents a request for payment, including details about payment-processing capabilities, the payment amount, and shipping information.

class PKRecurringPaymentRequest

A class that represents a request to set up a recurring payment, typically a subscription.

class PKAutomaticReloadPaymentRequest

A class that represents a request to set up an automatic reload payment, such as a store card top-up or a prepaid account.

class PKDeferredPaymentRequest

An object that represents a request to set up a deferred payment, such as a hotel booking or a pre-order.

