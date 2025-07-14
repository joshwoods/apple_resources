

- PassKit (Apple Pay and Wallet)
- PKPaymentInformationRequestHandling
-  handle(\_:completion:) 

Instance Method

# handle(\_:completion:)

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOSvisionOS 1.0+watchOS 7.0+

``` source
func handle(
    _ signatureRequest: PKBarcodeEventSignatureRequest,
    completion: @escaping PKSignatureRequestCompletionBlock
)
```

``` source
func handle(_ signatureRequest: PKBarcodeEventSignatureRequest) async -> PKBarcodeEventSignatureResponse
```

**Required**

## See Also

### Signing the transaction

class PKBarcodeEventSignatureRequest

class PKBarcodeEventSignatureResponse

typealias PKSignatureRequestCompletionBlock

