

- PassKit (Apple Pay and Wallet)
- PKAddPaymentPassRequestConfiguration
-  primaryAccountSuffix 

Instance Property

# primaryAccountSuffix

The last four or five digits of the card’s number.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOSvisionOS 1.0+

``` source
var primaryAccountSuffix: String? { get set }
```

## Discussion

The system prepends four dots to indicate that this is a partial number.

Note

Do not use the complete primary account number from the card. Use the last four or five digits only.

## See Also

### Payment pass request properties

var cardholderName: String?

The name of the person as shown on the card.

var encryptionScheme: PKEncryptionScheme

The encryption scheme to be used in this request.

struct PKEncryptionScheme

Encryption schemes.

var localizedDescription: String?

A short description of the card.

var cardDetails: [PKLabeledValue]

An array of labeled values that describe a card.

class PKLabeledValue

An object that can represent a detail about a payment card or other item.

var productIdentifiers: Set&lt;String>

var style: PKAddPaymentPassStyle

A value that indicates whether a pass is for access or for payment use.

enum PKAddPaymentPassStyle

The type of payment pass.

