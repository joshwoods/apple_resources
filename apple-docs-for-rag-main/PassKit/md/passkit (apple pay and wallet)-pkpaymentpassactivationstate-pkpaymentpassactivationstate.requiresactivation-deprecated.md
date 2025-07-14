

- PassKit (Apple Pay and Wallet)
- PKPaymentPassActivationState
-  PKPaymentPassActivationState.requiresActivation Deprecated

Case

# PKPaymentPassActivationState.requiresActivation

Not active but may be activated by the issuer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0–15.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 3.0–9.0Deprecated

``` source
case requiresActivation
```

Deprecated

Use PKSecureElementPass.PassActivationState.requiresActivation instead.

## See Also

### Activation states

case activated

Active and ready for payment use.

Deprecated

case activating

Not ready for use but activation is in progress.

Deprecated

case suspended

Not active and can’t be activated.

Deprecated

case deactivated

Not active because the issuer disabled the account associated with the device.

Deprecated

