

- PassKit (Apple Pay and Wallet)
- PKAddPaymentPassRequestConfiguration
-  style 

Instance Property

# style

A value that indicates whether a pass is for access or for payment use.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOSvisionOS 1.0+

``` source
var style: PKAddPaymentPassStyle { get set }
```

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

var primaryAccountSuffix: String?

The last four or five digits of the card’s number.

var cardDetails: [PKLabeledValue]

An array of labeled values that describe a card.

class PKLabeledValue

An object that can represent a detail about a payment card or other item.

var productIdentifiers: Set&lt;String>

enum PKAddPaymentPassStyle

The type of payment pass.

