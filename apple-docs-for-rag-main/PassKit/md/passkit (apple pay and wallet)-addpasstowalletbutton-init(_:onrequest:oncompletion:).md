

- PassKit (Apple Pay and Wallet)
- AddPassToWalletButton
-  init(\_:onRequest:onCompletion:) 

Initializer

# init(\_:onRequest:onCompletion:)

PassKitSwiftUIiOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
@MainActor @preconcurrency
init(
    _ configuration: PKAddPaymentPassRequestConfiguration,
    onRequest: @escaping (AddPassToWalletButtonResponse) async -> PKAddPaymentPassRequest,
    onCompletion: @escaping (Result) -> Void
)
```

Available when `Fallback` is `EmptyView`.

## See Also

### Creating the button

init(PKEncryptionScheme, cardholderName: String, passStyle: PKAddPaymentPassStyle, primaryAccountSuffix: String?, cardDetails: [PKLabeledValue]?, description: String?, filters: [AddPassToWalletButtonFilter], onRequest: (AddPassToWalletButtonResponse) async -> PKAddPaymentPassRequest, onCompletion: (Result&lt;PKSecureElementPass, any Error>) -> Void)

init(PKEncryptionScheme, cardholderName: String, passStyle: PKAddPaymentPassStyle, primaryAccountSuffix: String?, cardDetails: [PKLabeledValue]?, description: String?, filters: [AddPassToWalletButtonFilter], onRequest: (AddPassToWalletButtonResponse) async -> PKAddPaymentPassRequest, onCompletion: (Result&lt;PKSecureElementPass, any Error>) -> Void, fallback: () -> Fallback)

init([PKPass], onCompletion: (Bool) -> Void)

init(PKAddSecureElementPassConfiguration, onCompletion: (Result&lt;[PKSecureElementPass], any Error>) -> Void)

init([PKPass], onCompletion: (Bool) -> Void, fallback: () -> Fallback)

init(PKAddSecureElementPassConfiguration, onCompletion: (Result&lt;[PKSecureElementPass], any Error>) -> Void, fallback: () -> Fallback)

init(PKAddPaymentPassRequestConfiguration, onRequest: (AddPassToWalletButtonResponse) async -> PKAddPaymentPassRequest, onCompletion: (Result&lt;PKSecureElementPass, any Error>) -> Void, fallback: () -> Fallback)

init(PKEncryptionScheme, primaryAccountSuffix: String, passStyle: PKAddPaymentPassStyle, cardDetails: [PKLabeledValue]?, description: String?, filters: [AddPassToWalletButtonFilter], onRequest: (AddPassToWalletButtonResponse) async -> PKAddPaymentPassRequest, onCompletion: (Result&lt;PKSecureElementPass, any Error>) -> Void)

init(PKEncryptionScheme, primaryAccountSuffix: String, passStyle: PKAddPaymentPassStyle, cardDetails: [PKLabeledValue]?, description: String?, filters: [AddPassToWalletButtonFilter], onRequest: (AddPassToWalletButtonResponse) async -> PKAddPaymentPassRequest, onCompletion: (Result&lt;PKSecureElementPass, any Error>) -> Void, fallback: () -> Fallback)

init(action: () -> Void)

init(carKeyPassword: String, supportedRadioTechnologies: PKRadioTechnology, issuerIdentifier: String, onCompletion: (Result&lt;PKSecureElementPass, any Error>) -> Void)

init(carKeyPassword: String, supportedRadioTechnologies: PKRadioTechnology, issuerIdentifier: String, onCompletion: (Result&lt;PKSecureElementPass, any Error>) -> Void, fallback: () -> Fallback)

