

- PassKit (Apple Pay and Wallet)
- PayWithApplePayButton
-  init(\_:request:onPaymentAuthorizationChange:fallback:) 

Initializer

# init(\_:request:onPaymentAuthorizationChange:fallback:)

PassKitSwiftUIiOS 16.0+iPadOS 16.0+visionOSwatchOS 9.0+

``` source
nonisolated
init(
    _ label: PayWithApplePayButtonLabel = .plain,
    request: PKPaymentRequest,
    onPaymentAuthorizationChange: @escaping (PayWithApplePayButtonPaymentAuthorizationPhase) -> Void,
    @ViewBuilder fallback: () -> Fallback
)
```

Available when `Fallback` conforms to `View`.

## See Also

### Creating the button

init(PayWithApplePayButtonLabel, action: () -> Void)

init(PayWithApplePayButtonLabel, action: () -> Void, fallback: () -> Fallback)

init(PayWithApplePayButtonLabel, request: PKPaymentRequest, onPaymentAuthorizationChange: (PayWithApplePayButtonPaymentAuthorizationPhase) -> Void)

init(PayWithApplePayButtonLabel, request: PKPaymentRequest, onPaymentAuthorizationChange: (PayWithApplePayButtonPaymentAuthorizationPhase) -> Void, onMerchantSessionRequested: () async -> PKPaymentRequestMerchantSessionUpdate)

init(PayWithApplePayButtonLabel, request: PKPaymentRequest, onPaymentAuthorizationChange: (PayWithApplePayButtonPaymentAuthorizationPhase) -> Void, onMerchantSessionRequested: () async -> PKPaymentRequestMerchantSessionUpdate, fallback: () -> Fallback)

