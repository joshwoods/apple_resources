

- PassKit (Apple Pay and Wallet)
-  PKBarcodeEventMetadataRequest 

Class

# PKBarcodeEventMetadataRequest

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOSvisionOS 1.0+watchOS 7.0+

``` source
class PKBarcodeEventMetadataRequest
```

## Topics

### Getting QR Purchase Metadata

var deviceAccountIdentifier: String

var lastUsedBarcodeIdentifier: String

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

### Getting the transaction information

func handle(PKBarcodeEventConfigurationRequest, completion: () -> Void)

**Required**

func handleInformationRequest(PKBarcodeEventMetadataRequest, completion: PKInformationRequestCompletionBlock)

**Required**

class PKBarcodeEventConfigurationRequest

class PKBarcodeEventMetadataResponse

typealias PKInformationRequestCompletionBlock

