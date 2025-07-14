

- PassKit (Apple Pay and Wallet)
-  PKBarcodeEventSignatureResponse 

Class

# PKBarcodeEventSignatureResponse

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOSvisionOS 1.0+watchOS 7.0+

``` source
class PKBarcodeEventSignatureResponse
```

## Topics

### Creating a Signature Response

init(signedData: Data)

### Returning the Signature

var signedData: Data

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

class PKBarcodeEventSignatureRequest

typealias PKSignatureRequestCompletionBlock

