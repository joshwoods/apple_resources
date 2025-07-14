

- PassKit (Apple Pay and Wallet)
- PayWithApplePayButton
-  init(\_:request:onPaymentAuthorizationChange:) 

Initializer

# init(\_:request:onPaymentAuthorizationChange:)

PassKitSwiftUIiOS 16.0+iPadOS 16.0+visionOSwatchOS 9.0+

``` source
nonisolated
init(
    _ label: PayWithApplePayButtonLabel = .plain,
    request: PKPaymentRequest,
    onPaymentAuthorizationChange: @escaping (PayWithApplePayButtonPaymentAuthorizationPhase) -> Void
)
```

Available when `Fallback` is `EmptyView`.

## See Also

### Creating the button

init(PayWithApplePayButtonLabel, action: () -> Void)

init(PayWithApplePayButtonLabel, action: () -> Void, fallback: () -> Fallback)

init(PayWithApplePayButtonLabel, request: PKPaymentRequest, onPaymentAuthorizationChange: (PayWithApplePayButtonPaymentAuthorizationPhase) -> Void, fallback: () -> Fallback)

init(PayWithApplePayButtonLabel, request: PKPaymentRequest, onPaymentAuthorizationChange: (PayWithApplePayButtonPaymentAuthorizationPhase) -> Void, onMerchantSessionRequested: () async -> PKPaymentRequestMerchantSessionUpdate)

init(PayWithApplePayButtonLabel, request: PKPaymentRequest, onPaymentAuthorizationChange: (PayWithApplePayButtonPaymentAuthorizationPhase) -> Void, onMerchantSessionRequested: () async -> PKPaymentRequestMerchantSessionUpdate, fallback: () -> Fallback)

