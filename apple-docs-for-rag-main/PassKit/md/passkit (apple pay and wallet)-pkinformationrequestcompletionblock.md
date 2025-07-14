

- PassKit (Apple Pay and Wallet)
-  PKInformationRequestCompletionBlock 

Type Alias

# PKInformationRequestCompletionBlock

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
typealias PKInformationRequestCompletionBlock = (PKBarcodeEventMetadataResponse) -> Void
```

## See Also

### Getting the transaction information

func handle(PKBarcodeEventConfigurationRequest, completion: () -> Void)

**Required**

func handleInformationRequest(PKBarcodeEventMetadataRequest, completion: PKInformationRequestCompletionBlock)

**Required**

class PKBarcodeEventConfigurationRequest

class PKBarcodeEventMetadataRequest

class PKBarcodeEventMetadataResponse

