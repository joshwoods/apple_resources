

- PassKit (Apple Pay and Wallet)
- PKPaymentPass
-  activationState Deprecated

Instance Property

# activationState

The current activation state of the pass.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0–15.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 3.0–9.0Deprecated

``` source
var activationState: PKPaymentPassActivationState { get }
```

Deprecated

Use passActivationState instead.

## Discussion

You must activate a payment pass before you can use it.

For possible values and their meanings, see PKPaymentPass.

## See Also

### Related Documentation

Wallet Developer Guide

### Determining activation state

enum PKPaymentPassActivationState

Cases that indicate payment pass activation states.

Deprecated

