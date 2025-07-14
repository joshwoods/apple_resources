

- PassKit (Apple Pay and Wallet)
-  PKPaymentAuthorizationController 

Class

# PKPaymentAuthorizationController

An object that presents a sheet that prompts the user to authorize a payment request.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
class PKPaymentAuthorizationController
```

## Overview

After the user authorizes the payment request for a transaction, the delegate is called with a payment token used to authorize the transaction’s payment.

Important

The PKPaymentAuthorizationController class performs the same role as the PKPaymentAuthorizationViewController class, but it does not depend on the UIKit framework. This means that the authorization controller can be used in places where a view controller cannot (for example, in watchOS apps or in SiriKit extensions).

## Topics

### Creating a payment authorization controller

init(paymentRequest: PKPaymentRequest)

Initializes and returns a payment authorization controller.

convenience init(disbursementRequest: PKDisbursementRequest)

Creates a new payment authorization controller with the disbursement request you provide.

### Determining whether the user can make payments or disbursements

class func canMakePayments() -> Bool

Returns whether the user can make payments.

class func canMakePayments(usingNetworks: [PKPaymentNetwork]) -> Bool

Returns whether the user can make payments through the specified network.

class func canMakePayments(usingNetworks: [PKPaymentNetwork], capabilities: PKMerchantCapability) -> Bool

Returns whether the user can make payments using a card from the specified network with the specified capabilities.

class func supportsDisbursements() -> Bool

Returns a Boolean value that indicates whether this device can process disbursement requests.

class func supportsDisbursements(using: [PKPaymentNetwork]) -> Bool

Returns a Boolean value that indicates whether this device can process disbursement requests using the specified payment network brands.

class func supportsDisbursements(using: [PKPaymentNetwork], capabilities: PKMerchantCapability) -> Bool

Returns a Boolean value indicating whether this device can process disbursement requests using the specified payment network brands and capabilities.

### Handling user interactions

var delegate: (any PKPaymentAuthorizationControllerDelegate)?

The controller’s delegate.

protocol PKPaymentAuthorizationControllerDelegate

Methods that let you respond to user interactions with your payment authorization controller.

func present(completion: ((Bool) -> Void)?)

Presents the payment sheet modally over your app.

func dismiss(completion: (() -> Void)?)

Dismisses the payment sheet.

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

### Apple Pay availability

class PKPaymentAuthorizationViewController

An object that presents a sheet that prompts the user to authorize a payment request.

