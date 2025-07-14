

- PassKit (Apple Pay and Wallet)
- PKPassLibrary
-  isSecureElementPassActivationAvailable 

Instance Property

# isSecureElementPassActivationAvailable

A Boolean value that indicates whether the device supports creating Secure Element passes.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.12+visionOS 1.0+watchOS 6.2+

``` source
var isSecureElementPassActivationAvailable: Bool { get }
```

## Discussion

Secure Element pass activation requires a special entitlement that Apple provides. If the entitlement isn’t present, this property’s value is false.

## See Also

### Managing passes

func activate(PKSecureElementPass, activationData: Data, completion: ((Bool, (any Error)?) -> Void)?)

Activates a Secure Element pass using the specified data.

func replacePass(with: PKPass) -> Bool

Replaces a pass in the user’s pass library with the specified pass.

func removePass(PKPass)

Removes the pass from the user’s pass library.

