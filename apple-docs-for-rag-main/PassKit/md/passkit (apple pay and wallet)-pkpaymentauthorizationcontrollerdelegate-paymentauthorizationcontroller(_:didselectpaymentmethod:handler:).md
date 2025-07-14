

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationControllerDelegate
-  paymentAuthorizationController(\_:didSelectPaymentMethod:handler:) 

Instance Method

# paymentAuthorizationController(\_:didSelectPaymentMethod:handler:)

Tells the delegate that the user changed the payment method, and asks for an updated payment request.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
@MainActor
optional func paymentAuthorizationController(
    _ controller: PKPaymentAuthorizationController,
    didSelectPaymentMethod paymentMethod: PKPaymentMethod,
    handler completion: @escaping (PKPaymentRequestPaymentMethodUpdate) -> Void
)
```

``` source
@MainActor
optional func paymentAuthorizationController(
    _ controller: PKPaymentAuthorizationController,
    didSelectPaymentMethod paymentMethod: PKPaymentMethod
) async -> PKPaymentRequestPaymentMethodUpdate
```

## Parameters 

`controller`  

The payment authorization controller.

`paymentMethod`  

The selected payment method.

`completion`  

The completion handler to call with the updated payment summary items.

## Discussion

The system calls this method when the user selects a payment card. Use this delegate callback to update the summary items in response to the card type changing (for example, applying credit card surcharges), and then call the completion handler with the updated summary items.

## See Also

### Handling user’s payment method selection

func paymentAuthorizationController(PKPaymentAuthorizationController, didSelectPaymentMethod: PKPaymentMethod, completion: ([PKPaymentSummaryItem]) -> Void)

Tells the delegate that the user changed the payment method, and asks for an updated payment request.

Deprecated

