

- PassKit (Apple Pay and Wallet)
- Wallet
- PKPassLibrary
-  Deprecated Symbols 

API Collection

# Deprecated Symbols

Review unsupported symbols and their replacements.

## Topics

### Deprecated Methods

func activate(PKPaymentPass, withActivationCode: String, completion: ((Bool, any Error) -> Void)?)

Activates a payment pass using the provided activation code.

Deprecated

func activate(PKPaymentPass, withActivationData: Data, completion: ((Bool, any Error) -> Void)?)

Activates a payment pass using the provided activation code.

Deprecated

func canAddPaymentPass(withPrimaryAccountIdentifier: String) -> Bool

A Boolean value that indicates whether the app can add a card to Apple Pay for the provided primary account identifier.

Deprecated

class func isPaymentPassActivationAvailable() -> Bool

Returns a Boolean value that indicates whether the device supports adding payment passes.

Deprecated

func isPaymentPassActivationAvailable() -> Bool

Returns a Boolean value that indicates whether the device supports adding payment passes.

Deprecated

func present(PKPaymentPass)

Presents the payment pass for use in-store.

Deprecated

func remotePaymentPasses() -> [PKPaymentPass]

Returns a list of passes from a remote device.

Deprecated

