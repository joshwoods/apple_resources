

- PassKit (Apple Pay and Wallet)
-  PKBarcodeEventConfigurationRequest 

Class

# PKBarcodeEventConfigurationRequest

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOSvisionOS 1.0+watchOS 7.0+

``` source
class PKBarcodeEventConfigurationRequest
```

## Topics

### Reading Configuration Information

var deviceAccountIdentifier: String

var configurationDataType: PKBarcodeEventConfigurationDataType

var configurationData: Data

enum PKBarcodeEventConfigurationDataType

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

class PKBarcodeEventMetadataRequest

class PKBarcodeEventMetadataResponse

typealias PKInformationRequestCompletionBlock

