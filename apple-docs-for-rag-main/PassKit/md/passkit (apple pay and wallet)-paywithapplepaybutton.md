

- PassKit (Apple Pay and Wallet)
-  PayWithApplePayButton 

Structure

# PayWithApplePayButton

PassKitSwiftUIiOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+visionOSwatchOS 9.0+

``` source
@MainActor @preconcurrency
struct PayWithApplePayButton where Fallback : View
```

## Topics

### Creating the button

init(PayWithApplePayButtonLabel, action: () -> Void)

init(PayWithApplePayButtonLabel, action: () -> Void, fallback: () -> Fallback)

init(PayWithApplePayButtonLabel, request: PKPaymentRequest, onPaymentAuthorizationChange: (PayWithApplePayButtonPaymentAuthorizationPhase) -> Void)

init(PayWithApplePayButtonLabel, request: PKPaymentRequest, onPaymentAuthorizationChange: (PayWithApplePayButtonPaymentAuthorizationPhase) -> Void, fallback: () -> Fallback)

init(PayWithApplePayButtonLabel, request: PKPaymentRequest, onPaymentAuthorizationChange: (PayWithApplePayButtonPaymentAuthorizationPhase) -> Void, onMerchantSessionRequested: () async -> PKPaymentRequestMerchantSessionUpdate)

init(PayWithApplePayButtonLabel, request: PKPaymentRequest, onPaymentAuthorizationChange: (PayWithApplePayButtonPaymentAuthorizationPhase) -> Void, onMerchantSessionRequested: () async -> PKPaymentRequestMerchantSessionUpdate, fallback: () -> Fallback)

## Relationships

### Conforms To

- Sendable
- View

## See Also

### Apple Pay buttons

class PKPaymentButton

An object that displays a button either to trigger payments through Apple Pay or to prompt the user to set up a card.

struct PayWithApplePayButtonLabel

struct PayWithApplePayButtonStyle

