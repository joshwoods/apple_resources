

- PassKit (Apple Pay and Wallet)
- PKPassLibrary
-  removePass(\_:) 

Instance Method

# removePass(\_:)

Removes the pass from the user’s pass library.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0+watchOS 3.0+

``` source
func removePass(_ pass: PKPass)
```

## Parameters 

`pass`  

The pass to remove.

## Discussion

This method does nothing if your app doesn’t have the appropriate entitlement.

A user must confirm adding a pass to Wallet so only remove the pass in response to a user action, such as responding to a prompt to remove the pass or an app setting.

## See Also

### Managing passes

var isSecureElementPassActivationAvailable: Bool

A Boolean value that indicates whether the device supports creating Secure Element passes.

func activate(PKSecureElementPass, activationData: Data, completion: ((Bool, (any Error)?) -> Void)?)

Activates a Secure Element pass using the specified data.

func replacePass(with: PKPass) -> Bool

Replaces a pass in the user’s pass library with the specified pass.

