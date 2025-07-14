

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationViewControllerDelegate
-  paymentAuthorizationViewController(\_:didRequestMerchantSessionUpdate:) 

Instance Method

# paymentAuthorizationViewController(\_:didRequestMerchantSessionUpdate:)

Requests an object that validates the identity of a merchant for a payment request.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
optional func paymentAuthorizationViewController(
    _ controller: PKPaymentAuthorizationViewController,
    didRequestMerchantSessionUpdate handler: @escaping (PKPaymentRequestMerchantSessionUpdate) -> Void
)
```

``` source
optional func paymentAuthorizationViewControllerDidRequestMerchantSessionUpdate(controller: PKPaymentAuthorizationViewController) async -> PKPaymentRequestMerchantSessionUpdate
```

## Parameters 

`controller`  

The payment authorization view controller.

`handler`  

The completion handler to call with the updated merchant session.

## See Also

### Handling user’s payment authorization

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

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didSelect: PKPaymentMethod, handler: (PKPaymentRequestPaymentMethodUpdate) -> Void)

Tells the delegate that the user changed the payment method, and asks for an updated payment request.

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didSelect: PKPaymentMethod, completion: ([PKPaymentSummaryItem]) -> Void)

Tells the delegate that the user changed the payment method, and asks for an updated payment request.

Deprecated

