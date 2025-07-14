

- PassKit (Apple Pay and Wallet)
-  PKPaymentPassActivationState Deprecated

Enumeration

# PKPaymentPassActivationState

Cases that indicate payment pass activation states.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0–15.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 3.0–9.0Deprecated

``` source
enum PKPaymentPassActivationState
```

Deprecated

Use PKSecureElementPass.PassActivationState instead.

## Topics

### Activation states

case activated

Active and ready for payment use.

case requiresActivation

Not active but may be activated by the issuer.

case activating

Not ready for use but activation is in progress.

case suspended

Not active and can’t be activated.

case deactivated

Not active because the issuer disabled the account associated with the device.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Determining activation state

var activationState: PKPaymentPassActivationState

The current activation state of the pass.

Deprecated

