

- PassKit (Apple Pay and Wallet)
- PKPassLibrary
-  remotePaymentPasses() Deprecated

Instance Method

# remotePaymentPasses()

Returns a list of passes from a remote device.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
func remotePaymentPasses() -> [PKPaymentPass]
```

Deprecated

Use remoteSecureElementPasses instead.

## Return Value

An array that contains all the passes on a remote paired device (for example, an Apple Watch) for the current device.

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

class func isPaymentPassActivationAvailable() -> Bool

Returns a Boolean value that indicates whether the device supports adding payment passes.

Deprecated

func isPaymentPassActivationAvailable() -> Bool

Returns a Boolean value that indicates whether the device supports adding payment passes.

Deprecated

func present(PKPaymentPass)

Presents the payment pass for use in-store.

Deprecated

