

- PassKit (Apple Pay and Wallet)
- PKPaymentPassActivationState
-  PKPaymentPassActivationState.deactivated Deprecated

Case

# PKPaymentPassActivationState.deactivated

Not active because the issuer disabled the account associated with the device.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0–15.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 3.0–9.0Deprecated

``` source
case deactivated
```

Deprecated

Use PKSecureElementPass.PassActivationState.deactivated instead.

## Discussion

To reactivate the account, reprovision the pass.

## See Also

### Activation states

case activated

Active and ready for payment use.

Deprecated

case requiresActivation

Not active but may be activated by the issuer.

Deprecated

case activating

Not ready for use but activation is in progress.

Deprecated

case suspended

Not active and can’t be activated.

Deprecated

