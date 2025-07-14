

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationControllerDelegate
-  paymentAuthorizationController(\_:didSelectPaymentMethod:completion:) Deprecated

Instance Method

# paymentAuthorizationController(\_:didSelectPaymentMethod:completion:)

Tells the delegate that the user changed the payment method, and asks for an updated payment request.

iOS 10.0–11.0DeprecatediPadOS 10.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 11.0+visionOS 1.0–1.0DeprecatedwatchOS 3.0–4.0Deprecated

**iOS, iPadOS, Mac Catalyst, macOS, visionOS, watchOS**

``` source
optional func paymentAuthorizationController(
    _ controller: PKPaymentAuthorizationController,
    didSelectPaymentMethod paymentMethod: PKPaymentMethod,
    completion: @escaping ([PKPaymentSummaryItem]) -> Void
)
```

**Mac Catalyst, macOS, visionOS**

``` source
optional func paymentAuthorizationController(
    _ controller: PKPaymentAuthorizationController,
    didSelectPaymentMethod paymentMethod: PKPaymentMethod
) async -> [PKPaymentSummaryItem]
```

Deprecated

Use paymentAuthorizationController(_:didSelectPaymentMethod:handler:) instead.

## Parameters 

`controller`  

The payment authorization controller.

`paymentMethod`  

The new payment method.

`completion`  

The completion block to call with the updated payment summary items.

This block takes the following parameters:

`summaryItems`  
An updated array of summary items that include any changes due to fees or credit card surcharges associated with the payment method.

## Discussion

This method is called when the user has selected a new payment card. Use this delegate callback to update the summary items in response to the card type changing (for example, applying credit card surcharges), and then call the callback with the updated summary items.

Note

The delegate receives no further callbacks except paymentAuthorizationControllerDidFinish(_:) until it has invoked the completion block.

## See Also

### Handling user’s payment method selection

func paymentAuthorizationController(PKPaymentAuthorizationController, didSelectPaymentMethod: PKPaymentMethod, handler: (PKPaymentRequestPaymentMethodUpdate) -> Void)

Tells the delegate that the user changed the payment method, and asks for an updated payment request.

