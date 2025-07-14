

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationViewControllerDelegate
-  paymentAuthorizationViewControllerDidFinish(\_:) 

Instance Method

# paymentAuthorizationViewControllerDidFinish(\_:)

Tells the delegate that payment authorization finished.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+

``` source
func paymentAuthorizationViewControllerDidFinish(_ controller: PKPaymentAuthorizationViewController)
```

**Required**

## Parameters 

`controller`  

The payment authorization view controller.

## Discussion

This delegate method is called every time a payment finishes. A payment may finish because authorization was completed in paymentAuthorizationViewController(_:didAuthorizePayment:handler:), because authorization timed out, or because the user canceled the payment.

Important

Make any needed payment-related updates to your app’s state in this delegate method, especially if the payment is canceled or times out. Also, be sure to call dismiss(completion:) on the payment authorization view controller.

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

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didSelect: PKPaymentMethod, handler: (PKPaymentRequestPaymentMethodUpdate) -> Void)

Tells the delegate that the user changed the payment method, and asks for an updated payment request.

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didSelect: PKPaymentMethod, completion: ([PKPaymentSummaryItem]) -> Void)

Tells the delegate that the user changed the payment method, and asks for an updated payment request.

Deprecated

