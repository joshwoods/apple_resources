

- PassKit (Apple Pay and Wallet)
-  PKBarcodeEventMetadataResponse 

Class

# PKBarcodeEventMetadataResponse

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOSvisionOS 1.0+watchOS 7.0+

``` source
class PKBarcodeEventMetadataResponse
```

## Topics

### Creating an Event Metadata Response

init(paymentInformation: Data)

### Getting QR Payment Information

var paymentInformation: Data

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

class PKBarcodeEventMetadataRequest

typealias PKInformationRequestCompletionBlock

