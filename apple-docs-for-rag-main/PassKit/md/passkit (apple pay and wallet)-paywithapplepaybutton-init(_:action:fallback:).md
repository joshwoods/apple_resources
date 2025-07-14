

- PassKit (Apple Pay and Wallet)
- PayWithApplePayButton
-  init(\_:action:fallback:) 

Initializer

# init(\_:action:fallback:)

PassKitSwiftUIiOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+visionOSwatchOS 9.0+

``` source
nonisolated
init(
    _ label: PayWithApplePayButtonLabel = .plain,
    action: @escaping () -> Void,
    @ViewBuilder fallback: () -> Fallback
)
```

## See Also

### Creating the button

init(PayWithApplePayButtonLabel, action: () -> Void)

init(PayWithApplePayButtonLabel, request: PKPaymentRequest, onPaymentAuthorizationChange: (PayWithApplePayButtonPaymentAuthorizationPhase) -> Void)

init(PayWithApplePayButtonLabel, request: PKPaymentRequest, onPaymentAuthorizationChange: (PayWithApplePayButtonPaymentAuthorizationPhase) -> Void, fallback: () -> Fallback)

init(PayWithApplePayButtonLabel, request: PKPaymentRequest, onPaymentAuthorizationChange: (PayWithApplePayButtonPaymentAuthorizationPhase) -> Void, onMerchantSessionRequested: () async -> PKPaymentRequestMerchantSessionUpdate)

init(PayWithApplePayButtonLabel, request: PKPaymentRequest, onPaymentAuthorizationChange: (PayWithApplePayButtonPaymentAuthorizationPhase) -> Void, onMerchantSessionRequested: () async -> PKPaymentRequestMerchantSessionUpdate, fallback: () -> Fallback)

