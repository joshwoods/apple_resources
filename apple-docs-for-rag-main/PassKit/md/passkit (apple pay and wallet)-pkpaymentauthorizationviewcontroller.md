

- PassKit (Apple Pay and Wallet)
-  PKPaymentAuthorizationViewController 

Class

# PKPaymentAuthorizationViewController

An object that presents a sheet that prompts the user to authorize a payment request.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+

``` source
@MainActor
class PKPaymentAuthorizationViewController
```

## Overview

After the user authorizes the payment request for a transaction, the delegate is called with a payment token used to authorize the transaction’s payment.

## Topics

### Determining whether the user can make payments

class func canMakePayments() -> Bool

Returns whether the user can make payments.

class func canMakePayments(usingNetworks: [PKPaymentNetwork]) -> Bool

Returns whether the user can make payments through the specified network.

class func canMakePayments(usingNetworks: [PKPaymentNetwork], capabilities: PKMerchantCapability) -> Bool

Returns whether the user can make payments using a card from the specified network with the specified capabilities.

class func supportsDisbursements() -> Bool

Returns a Boolean value that indicates whether this device can process disbursement requests.

class func supportsDisbursements(using: [PKPaymentNetwork]) -> Bool

Returns a Boolean value that indicates whether this device can process disbursement requests using the specified payment networks.

class func supportsDisbursements(using: [PKPaymentNetwork], capabilities: PKMerchantCapability) -> Bool

Returns a Boolean value that indicates whether this device can process disbursement requests using the specified payment networks and merchant capabilities.

### Handling user interactions

var delegate: (any PKPaymentAuthorizationViewControllerDelegate)?

The view controller’s delegate.

protocol PKPaymentAuthorizationViewControllerDelegate

Methods that let you respond to user interactions with your payment authorization view controller.

### Creating a payment authorization view controller

init?(paymentRequest: PKPaymentRequest)

Initializes and returns a payment authorization view controller.

convenience init(disbursementRequest: PKDisbursementRequest)

Initializes and returns a new payment authorization view controller with the provided disbursement request.

## Relationships

### Inherits From

- NSViewController
- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSEditor
- NSExtensionRequestHandling
- NSObjectProtocol
- NSSeguePerforming
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Apple Pay availability

class PKPaymentAuthorizationController

An object that presents a sheet that prompts the user to authorize a payment request.

