

- StoreKit
-  SKPaymentDiscount Deprecated

Class

# SKPaymentDiscount

The signed discount to apply to a payment.

iOS 12.2–18.0DeprecatediPadOS 12.2–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.14.4–15.0DeprecatedtvOS 12.2–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
class SKPaymentDiscount
```

Deprecated

Create a Product.PurchaseOption.promotionalOffer to use in Product.purchase(confirmIn:options:)

## Mentioned in 

Implementing promotional offers in your app

Generating a signature for promotional offers

## Overview

The SKPaymentDiscount contains the details of a promotional offer discount that you want to apply to a SKMutablePayment.

Include the signature that you generated in this object. For guidance, see Generating a signature for promotional offers. The App Store uses this signature and the parameters to validate the promotional offer. Keep in mind that the signature must correspond to the parameters in the payment for a transaction to be successful.

## Topics

### Initializing a Payment Discount

init(identifier: String, keyIdentifier: String, nonce: UUID, signature: String, timestamp: NSNumber)

Initializes the payment discount with a signature and the parameters used by the signature.

### Identifying the Discount

var identifier: String

A string used to uniquely identify a discount offer for a product.

var keyIdentifier: String

A string that identifies the key used to generate the signature.

### Validating the Discount

var nonce: UUID

A universally unique ID (UUID) value that you define.

var signature: String

A string representing the properties of a specific promotional offer, cryptographically signed.

var timestamp: NSNumber

The date and time of the signature’s creation in milliseconds, formatted in Unix epoch time.

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

### Getting Discount Details

var paymentDiscount: SKPaymentDiscount?

The details of the discount offer to apply to the payment.

Deprecated

