

- PassKit (Apple Pay and Wallet)
-  PKAddPaymentPassRequestConfiguration 

Class

# PKAddPaymentPassRequestConfiguration

Contains the configuration data for a view controller that lets the user add a payment pass.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOSvisionOS 1.0+

``` source
class PKAddPaymentPassRequestConfiguration
```

## Overview

The encryption scheme, cardholder name, and primary account suffix are required for configuration. The configuration information is used for setup and display only. It should not contain any sensitive information.

Important

Adding payment passes requires a special entitlement issued by Apple. Your app must include this entitlement before you can use this class. For more information on requesting this entitlement, see the Card Issuers section at developer.apple.com/apple-pay/.

## Topics

### Creating a request configuration

init?(encryptionScheme: PKEncryptionScheme)

Instantiates a new request configuration with the given encryption scheme.

struct PKEncryptionScheme

Encryption schemes.

### Filtering pass libraries

var paymentNetwork: PKPaymentNetwork?

The payment network.

var primaryAccountIdentifier: String?

A primary account identifier, used to filter out pass libraries.

var requiresFelicaSecureElement: Bool

A Boolean value that indicates whether the payment pass requires the Felica Secure Element.

### Payment pass request properties

var cardholderName: String?

The name of the person as shown on the card.

var encryptionScheme: PKEncryptionScheme

The encryption scheme to be used in this request.

struct PKEncryptionScheme

Encryption schemes.

var localizedDescription: String?

A short description of the card.

var primaryAccountSuffix: String?

The last four or five digits of the card’s number.

var cardDetails: [PKLabeledValue]

An array of labeled values that describe a card.

class PKLabeledValue

An object that can represent a detail about a payment card or other item.

var productIdentifiers: Set&lt;String>

var style: PKAddPaymentPassStyle

A value that indicates whether a pass is for access or for payment use.

enum PKAddPaymentPassStyle

The type of payment pass.

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

### Creating an add-payment-pass view controller

init?(requestConfiguration: PKAddPaymentPassRequestConfiguration, delegate: (any PKAddPaymentPassViewControllerDelegate)?)

Returns an initialized add payment view controller object, using the provided configuration and delegate.

