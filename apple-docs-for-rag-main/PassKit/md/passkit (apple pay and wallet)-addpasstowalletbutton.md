

- PassKit (Apple Pay and Wallet)
-  AddPassToWalletButton 

Structure

# AddPassToWalletButton

PassKitSwiftUIiOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
@MainActor @preconcurrency
struct AddPassToWalletButton where Fallback : View
```

## Topics

### Creating the button

init(PKEncryptionScheme, cardholderName: String, passStyle: PKAddPaymentPassStyle, primaryAccountSuffix: String?, cardDetails: [PKLabeledValue]?, description: String?, filters: [AddPassToWalletButtonFilter], onRequest: (AddPassToWalletButtonResponse) async -> PKAddPaymentPassRequest, onCompletion: (Result&lt;PKSecureElementPass, any Error>) -> Void)

init(PKEncryptionScheme, cardholderName: String, passStyle: PKAddPaymentPassStyle, primaryAccountSuffix: String?, cardDetails: [PKLabeledValue]?, description: String?, filters: [AddPassToWalletButtonFilter], onRequest: (AddPassToWalletButtonResponse) async -> PKAddPaymentPassRequest, onCompletion: (Result&lt;PKSecureElementPass, any Error>) -> Void, fallback: () -> Fallback)

init([PKPass], onCompletion: (Bool) -> Void)

init(PKAddSecureElementPassConfiguration, onCompletion: (Result&lt;[PKSecureElementPass], any Error>) -> Void)

init([PKPass], onCompletion: (Bool) -> Void, fallback: () -> Fallback)

init(PKAddSecureElementPassConfiguration, onCompletion: (Result&lt;[PKSecureElementPass], any Error>) -> Void, fallback: () -> Fallback)

init(PKAddPaymentPassRequestConfiguration, onRequest: (AddPassToWalletButtonResponse) async -> PKAddPaymentPassRequest, onCompletion: (Result&lt;PKSecureElementPass, any Error>) -> Void)

init(PKAddPaymentPassRequestConfiguration, onRequest: (AddPassToWalletButtonResponse) async -> PKAddPaymentPassRequest, onCompletion: (Result&lt;PKSecureElementPass, any Error>) -> Void, fallback: () -> Fallback)

init(PKEncryptionScheme, primaryAccountSuffix: String, passStyle: PKAddPaymentPassStyle, cardDetails: [PKLabeledValue]?, description: String?, filters: [AddPassToWalletButtonFilter], onRequest: (AddPassToWalletButtonResponse) async -> PKAddPaymentPassRequest, onCompletion: (Result&lt;PKSecureElementPass, any Error>) -> Void)

init(PKEncryptionScheme, primaryAccountSuffix: String, passStyle: PKAddPaymentPassStyle, cardDetails: [PKLabeledValue]?, description: String?, filters: [AddPassToWalletButtonFilter], onRequest: (AddPassToWalletButtonResponse) async -> PKAddPaymentPassRequest, onCompletion: (Result&lt;PKSecureElementPass, any Error>) -> Void, fallback: () -> Fallback)

init(action: () -> Void)

init(carKeyPassword: String, supportedRadioTechnologies: PKRadioTechnology, issuerIdentifier: String, onCompletion: (Result&lt;PKSecureElementPass, any Error>) -> Void)

init(carKeyPassword: String, supportedRadioTechnologies: PKRadioTechnology, issuerIdentifier: String, onCompletion: (Result&lt;PKSecureElementPass, any Error>) -> Void, fallback: () -> Fallback)

## Relationships

### Conforms To

- Sendable
- View

## See Also

### Common objects

class PKObject

An opaque type that acts as the superclass for the pass object.

class PKAddPassButton

Provides a button that enables users to add passes to Wallet.

class PKLabeledValue

An object that can represent a detail about a payment card or other item.

struct AddPassToWalletButtonFilter

struct AddPassToWalletButtonResponse

struct AddPassToWalletButtonStyle

