

- PassKit (Apple Pay and Wallet)
- PKPassLibrary
-  isPaymentPassActivationAvailable() Deprecated

Type Method

# isPaymentPassActivationAvailable()

Returns a Boolean value that indicates whether the device supports adding payment passes.

iOS 8.0–9.0DeprecatediPadOS 8.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12+visionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
class func isPaymentPassActivationAvailable() -> Bool
```

Deprecated

Use isSecureElementPassActivationAvailable instead.

## Return Value

true if the device supports adding payment passes.

## See Also

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

func isPaymentPassActivationAvailable() -> Bool

Returns a Boolean value that indicates whether the device supports adding payment passes.

Deprecated

func present(PKPaymentPass)

Presents the payment pass for use in-store.

Deprecated

func remotePaymentPasses() -> [PKPaymentPass]

Returns a list of passes from a remote device.

Deprecated

