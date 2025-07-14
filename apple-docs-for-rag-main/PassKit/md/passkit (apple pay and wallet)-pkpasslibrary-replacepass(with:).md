

- PassKit (Apple Pay and Wallet)
- PKPassLibrary
-  replacePass(with:) 

Instance Method

# replacePass(with:)

Replaces a pass in the user’s pass library with the specified pass.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0+watchOS 3.0+

``` source
func replacePass(with pass: PKPass) -> Bool
```

## Parameters 

`pass`  

The new pass.

## Return Value

true if PassKit replaces the pass successfully; otherwise, false.

## Discussion

The new pass replaces the existing pass with the same pass type identifier and serial number. If there isn’t such a pass in the user’s pass library, the replacement fails.

## See Also

### Managing passes

var isSecureElementPassActivationAvailable: Bool

A Boolean value that indicates whether the device supports creating Secure Element passes.

func activate(PKSecureElementPass, activationData: Data, completion: ((Bool, (any Error)?) -> Void)?)

Activates a Secure Element pass using the specified data.

func removePass(PKPass)

Removes the pass from the user’s pass library.

