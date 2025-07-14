

- PassKit (Apple Pay and Wallet)
- PKSecureElementPass
- PKSecureElementPass.PassActivationState
-  PKSecureElementPass.PassActivationState.requiresActivation 

Case

# PKSecureElementPass.PassActivationState.requiresActivation

The pass requires activation by the issuer.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 11.0+visionOS 1.0+watchOS 6.2+

``` source
case requiresActivation
```

## See Also

### Activation states

case activating

The pass isn’t ready to use, but activation is in progress

case activated

The pass is active and ready to use.

case suspended

The user or the issuer has suspended the pass and it isn’t available to use.

case deactivated

The issuer has deactivated the pass.

