

- PassKit (Apple Pay and Wallet)
- PKPaymentInformationRequestHandling
-  handle(\_:completion:) 

Instance Method

# handle(\_:completion:)

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOSvisionOS 1.0+watchOS 7.0+

``` source
func handle(
    _ configurationRequest: PKBarcodeEventConfigurationRequest,
    completion: @escaping () -> Void
)
```

``` source
func handle(_ configurationRequest: PKBarcodeEventConfigurationRequest) async
```

**Required**

## See Also

### Getting the transaction information

func handleInformationRequest(PKBarcodeEventMetadataRequest, completion: PKInformationRequestCompletionBlock)

**Required**

class PKBarcodeEventConfigurationRequest

class PKBarcodeEventMetadataRequest

class PKBarcodeEventMetadataResponse

typealias PKInformationRequestCompletionBlock

