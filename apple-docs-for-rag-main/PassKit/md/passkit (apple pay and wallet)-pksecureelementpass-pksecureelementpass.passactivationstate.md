

- PassKit (Apple Pay and Wallet)
- PKSecureElementPass
-  PKSecureElementPass.PassActivationState 

Enumeration

# PKSecureElementPass.PassActivationState

The activation states of a Secure Element pass.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 11.0+visionOS 1.0+watchOS 6.2+

``` source
enum PassActivationState
```

## Topics

### Activation states

case requiresActivation

The pass requires activation by the issuer.

case activating

The pass isn’t ready to use, but activation is in progress

case activated

The pass is active and ready to use.

case suspended

The user or the issuer has suspended the pass and it isn’t available to use.

case deactivated

The issuer has deactivated the pass.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the activation state

var passActivationState: PKSecureElementPass.PassActivationState

The activation state of the pass.

