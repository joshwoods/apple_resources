

- PassKit (Apple Pay and Wallet)
- PayWithApplePayButton
-  init(\_:action:) 

Initializer

# init(\_:action:)

PassKitSwiftUIiOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+visionOSwatchOS 9.0+

``` source
nonisolated
init(
    _ label: PayWithApplePayButtonLabel = .plain,
    action: @escaping () -> Void
)
```

Available when `Fallback` is `EmptyView`.

## See Also

### Creating the button

init(PayWithApplePayButtonLabel, action: () -> Void, fallback: () -> Fallback)

init(PayWithApplePayButtonLabel, request: PKPaymentRequest, onPaymentAuthorizationChange: (PayWithApplePayButtonPaymentAuthorizationPhase) -> Void)

init(PayWithApplePayButtonLabel, request: PKPaymentRequest, onPaymentAuthorizationChange: (PayWithApplePayButtonPaymentAuthorizationPhase) -> Void, fallback: () -> Fallback)

init(PayWithApplePayButtonLabel, request: PKPaymentRequest, onPaymentAuthorizationChange: (PayWithApplePayButtonPaymentAuthorizationPhase) -> Void, onMerchantSessionRequested: () async -> PKPaymentRequestMerchantSessionUpdate)

init(PayWithApplePayButtonLabel, request: PKPaymentRequest, onPaymentAuthorizationChange: (PayWithApplePayButtonPaymentAuthorizationPhase) -> Void, onMerchantSessionRequested: () async -> PKPaymentRequestMerchantSessionUpdate, fallback: () -> Fallback)

