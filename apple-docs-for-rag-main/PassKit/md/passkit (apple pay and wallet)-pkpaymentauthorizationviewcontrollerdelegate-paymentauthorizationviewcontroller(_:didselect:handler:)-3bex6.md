

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationViewControllerDelegate
-  paymentAuthorizationViewController(\_:didSelect:handler:) 

Instance Method

# paymentAuthorizationViewController(\_:didSelect:handler:)

Tells the delegate that the user changed the payment method, and asks for an updated payment request.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+

``` source
optional func paymentAuthorizationViewController(
    _ controller: PKPaymentAuthorizationViewController,
    didSelect paymentMethod: PKPaymentMethod,
    handler completion: @escaping (PKPaymentRequestPaymentMethodUpdate) -> Void
)
```

``` source
optional func paymentAuthorizationViewController(
    _ controller: PKPaymentAuthorizationViewController,
    didSelect paymentMethod: PKPaymentMethod
) async -> PKPaymentRequestPaymentMethodUpdate
```

## Parameters 

`controller`  

The payment authorization view controller.

`paymentMethod`  

The new payment method.

`completion`  

The completion handler to call with the updated payment summary items.

## Discussion

The system calls this method when the user selects a new payment card. Use this delegate callback to update the summary items in response to the card type changing (for example, applying credit card surcharges), and then call the handler with the updated summary items.

## See Also

### Handling user’s payment authorization

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didRequestMerchantSessionUpdate: (PKPaymentRequestMerchantSessionUpdate) -> Void)

Requests an object that validates the identity of a merchant for a payment request.

func paymentAuthorizationViewControllerWillAuthorizePayment(PKPaymentAuthorizationViewController)

Tells the delegate that the user is authorizing the payment request.

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didAuthorizePayment: PKPayment, handler: (PKPaymentAuthorizationResult) -> Void)

Tells the delegate that the user authorized the payment request, and asks for a result.

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didAuthorizePayment: PKPayment, completion: (PKPaymentAuthorizationStatus) -> Void)

Tells the delegate that the user authorized the payment request, and asks for a result.

Deprecated

func paymentAuthorizationViewControllerDidFinish(PKPaymentAuthorizationViewController)

Tells the delegate that payment authorization finished.

**Required**

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didSelect: PKPaymentMethod, completion: ([PKPaymentSummaryItem]) -> Void)

Tells the delegate that the user changed the payment method, and asks for an updated payment request.

Deprecated

