

- PassKit (Apple Pay and Wallet)
- PKPassLibrary
-  activate(\_:activationData:completion:) 

Instance Method

# activate(\_:activationData:completion:)

Activates a Secure Element pass using the specified data.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.12+visionOS 1.0+

``` source
func activate(
    _ secureElementPass: PKSecureElementPass,
    activationData: Data,
    completion: ((Bool, (any Error)?) -> Void)? = nil
)
```

``` source
func activate(
    _ secureElementPass: PKSecureElementPass,
    activationData: Data
) async throws -> Bool
```

## Parameters 

`secureElementPass`  

The Secure Element pass to activate.

`activationData`  

A cryptographic value that the activation process requires.

`completion`  

A closure that PassKit executes after it attempts activation.

`success`  
A value that indicates whether activation is successful..

`error`  
If activation fails, an error that describes the failure; otherwise, otherwise, `nil` in Swift or null in Objective-C.

## Discussion

You must provision the Secure Element pass and make sure it’s in the PKSecureElementPass.PassActivationState.requiresActivation state before you call this method.

## See Also

### Managing passes

var isSecureElementPassActivationAvailable: Bool

A Boolean value that indicates whether the device supports creating Secure Element passes.

func replacePass(with: PKPass) -> Bool

Replaces a pass in the user’s pass library with the specified pass.

func removePass(PKPass)

Removes the pass from the user’s pass library.

