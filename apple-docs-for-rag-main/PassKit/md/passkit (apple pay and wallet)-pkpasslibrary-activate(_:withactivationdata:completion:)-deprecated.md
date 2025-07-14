

- PassKit (Apple Pay and Wallet)
- PKPassLibrary
-  activate(\_:withActivationData:completion:) Deprecated

Instance Method

# activate(\_:withActivationData:completion:)

Activates a payment pass using the provided activation code.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
func activate(
    _ paymentPass: PKPaymentPass,
    withActivationData activationData: Data,
    completion: ((Bool, any Error) -> Void)? = nil
)
```

Deprecated

Use activate(_:activationData:completion:) instead.

## Parameters 

`paymentPass`  

The payment pass to activate.

`activationData`  

The one-time cryptographic password.

PassKit encodes the data as Base64 and then sends it to the payment network. The framework treats this data as an opaque value.

`completion`  

The completion block that PassKit calls after activation.

This block takes the following parameters:

`success`  
true if the authorization succeeds; otherwise, false.

`error`  
If `success` is false, a description of the error.

## Discussion

You can only activate a provisioned pass, and it must be in the PKPaymentPassActivationState.requiresActivation state.

Important

Activating payment passes requires a special entitlement issued from Apple. For more information, see developer.apple.com/apple-pay/.

## See Also

### Deprecated Methods

func activate(PKPaymentPass, withActivationCode: String, completion: ((Bool, any Error) -> Void)?)

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

