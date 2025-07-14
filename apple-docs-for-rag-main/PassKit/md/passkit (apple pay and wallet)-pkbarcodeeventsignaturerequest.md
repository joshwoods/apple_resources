

- PassKit (Apple Pay and Wallet)
-  PKBarcodeEventSignatureRequest 

Class

# PKBarcodeEventSignatureRequest

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOSvisionOS 1.0+watchOS 7.0+

``` source
class PKBarcodeEventSignatureRequest
```

## Topics

### Getting Transaction Details

var amount: NSNumber

var currencyCode: String

var transactionDate: Date

var transactionIdentifier: String

var transactionStatus: String

var merchantName: String

var rawMerchantName: String

### Getting Signing Information

var partialSignature: Data

var barcodeIdentifier: String

var deviceAccountIdentifier: String

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

### Signing the transaction

func handle(PKBarcodeEventSignatureRequest, completion: PKSignatureRequestCompletionBlock)

**Required**

class PKBarcodeEventSignatureResponse

typealias PKSignatureRequestCompletionBlock

