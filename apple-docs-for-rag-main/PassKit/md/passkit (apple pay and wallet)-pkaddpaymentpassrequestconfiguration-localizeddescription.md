

- PassKit (Apple Pay and Wallet)
- PKAddPaymentPassRequestConfiguration
-  localizedDescription 

Instance Property

# localizedDescription

A short description of the card.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOSvisionOS 1.0+

``` source
var localizedDescription: String? { get set }
```

## Discussion

This property provides a user-visible description that clearly identifies the card.

## See Also

### Payment pass request properties

var cardholderName: String?

The name of the person as shown on the card.

var encryptionScheme: PKEncryptionScheme

The encryption scheme to be used in this request.

struct PKEncryptionScheme

Encryption schemes.

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

