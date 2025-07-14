

- PassKit (Apple Pay and Wallet)
- PKPaymentInformationRequestHandling
-  handleInformationRequest(\_:completion:) 

Instance Method

# handleInformationRequest(\_:completion:)

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOSvisionOS 1.0+watchOS 7.0+

``` source
func handleInformationRequest(
    _ infoRequest: PKBarcodeEventMetadataRequest,
    completion: @escaping PKInformationRequestCompletionBlock
)
```

``` source
func handleInformationRequest(_ infoRequest: PKBarcodeEventMetadataRequest) async -> PKBarcodeEventMetadataResponse
```

**Required**

## See Also

### Getting the transaction information

func handle(PKBarcodeEventConfigurationRequest, completion: () -> Void)

**Required**

class PKBarcodeEventConfigurationRequest

class PKBarcodeEventMetadataRequest

class PKBarcodeEventMetadataResponse

typealias PKInformationRequestCompletionBlock

