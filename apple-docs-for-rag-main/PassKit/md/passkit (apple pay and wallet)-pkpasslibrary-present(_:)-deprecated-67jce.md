

- PassKit (Apple Pay and Wallet)
- PKPassLibrary
-  present(\_:) Deprecated

Instance Method

# present(\_:)

Presents the payment pass for use in-store.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0–2.4Deprecated

``` source
func present(_ pass: PKPaymentPass)
```

Deprecated

Use present(_:) instead.

## Parameters 

`pass`  

The pass to present.

## Discussion

You can use present(_:) to present your payment pass for use in-store. Your app must have the proper entitlement to see the payment pass that you present. Therefore, this method is mostly relevant to a bank or merchant app that presents its own payment method for use in-store.

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

func remotePaymentPasses() -> [PKPaymentPass]

Returns a list of passes from a remote device.

Deprecated

