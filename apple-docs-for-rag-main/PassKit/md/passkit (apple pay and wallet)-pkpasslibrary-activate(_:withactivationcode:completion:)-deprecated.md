

- PassKit (Apple Pay and Wallet)
- PKPassLibrary
-  activate(\_:withActivationCode:completion:) Deprecated

Instance Method

# activate(\_:withActivationCode:completion:)

Activates a payment pass using the provided activation code.

iOS 8.0–9.0DeprecatediPadOS 8.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12+visionOS 1.0–1.0Deprecated

``` source
func activate(
    _ paymentPass: PKPaymentPass,
    withActivationCode activationCode: String,
    completion: ((Bool, any Error) -> Void)? = nil
)
```

Deprecated

Use activate(_:activationData:completion:) instead.

## Parameters 

`paymentPass`  

The payment pass to activate.

`activationCode`  

The activation code.

`completion`  

The completion block that PassKit calls after activation.

This block takes the following parameters:

`success`  
true if authorization succeeds; otherwise, false.

`error`  
If `success` is false, a description of the error.

## Discussion

You can only activate a provisioned pass, and it must be in the PKPaymentPassActivationState.requiresActivation state.

Important

Activating payment passes requires a special entitlement from Apple. For more information about requesting this entitlement, see developer.apple.com/apple-pay/.

## See Also

### Deprecated Methods

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

