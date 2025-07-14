

- PassKit (Apple Pay and Wallet)
- PKPassLibrary
-  canAddPaymentPass(withPrimaryAccountIdentifier:) Deprecated

Instance Method

# canAddPaymentPass(withPrimaryAccountIdentifier:)

A Boolean value that indicates whether the app can add a card to Apple Pay for the provided primary account identifier.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
func canAddPaymentPass(withPrimaryAccountIdentifier primaryAccountIdentifier: String) -> Bool
```

Deprecated

Use canAddSecureElementPass(primaryAccountIdentifier:) instead.

## Parameters 

`primaryAccountIdentifier`  

A unique identifier for the underlying funding primary account number (PAN). This isn’t the PAN itself.

## Return Value

true if PassKit can add the pass.

## Discussion

Adding payment passes requires a special entitlement from Apple. If the entitlement isn’t present, this method returns false. For more information about requesting this entitlement, see developer.apple.com/apple-pay/.

## See Also

### Deprecated Methods

func activate(PKPaymentPass, withActivationCode: String, completion: ((Bool, any Error) -> Void)?)

Activates a payment pass using the provided activation code.

Deprecated

func activate(PKPaymentPass, withActivationData: Data, completion: ((Bool, any Error) -> Void)?)

Activates a payment pass using the provided activation code.

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

