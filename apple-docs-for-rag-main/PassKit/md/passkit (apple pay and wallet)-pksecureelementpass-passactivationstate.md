

- PassKit (Apple Pay and Wallet)
- PKSecureElementPass
-  passActivationState 

Instance Property

# passActivationState

The activation state of the pass.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 11.0+visionOS 1.0+watchOS 6.2+

``` source
var passActivationState: PKSecureElementPass.PassActivationState { get }
```

## Discussion

You must activate a secure pass before it can be used.

For possible values and their meanings, see PKSecureElementPass.PassActivationState.

## See Also

### Getting the activation state

enum PassActivationState

The activation states of a Secure Element pass.

