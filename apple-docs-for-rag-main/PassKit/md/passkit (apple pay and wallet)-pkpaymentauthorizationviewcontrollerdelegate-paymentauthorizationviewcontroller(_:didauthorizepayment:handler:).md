

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationViewControllerDelegate
-  paymentAuthorizationViewController(\_:didAuthorizePayment:handler:) 

Instance Method

# paymentAuthorizationViewController(\_:didAuthorizePayment:handler:)

Tells the delegate that the user authorized the payment request, and asks for a result.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+

``` source
optional func paymentAuthorizationViewController(
    _ controller: PKPaymentAuthorizationViewController,
    didAuthorizePayment payment: PKPayment,
    handler completion: @escaping (PKPaymentAuthorizationResult) -> Void
)
```

``` source
optional func paymentAuthorizationViewController(
    _ controller: PKPaymentAuthorizationViewController,
    didAuthorizePayment payment: PKPayment
) async -> PKPaymentAuthorizationResult
```

## Parameters 

`controller`  

The payment authorization view controller.

`payment`  

The authorized payment. This object contains the payment token you need to submit to your payment processor, as well as the billing and shipping information required by the payment request.

`completion`  

The completion handler to call with the result of authorizing the payment.

## Discussion

The system calls this method after it authorizes the payment request. You submit the payment information to your payment processor to authorize the transaction, and then call the completion handler.

## See Also

### Handling user’s payment authorization

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didRequestMerchantSessionUpdate: (PKPaymentRequestMerchantSessionUpdate) -> Void)

Requests an object that validates the identity of a merchant for a payment request.

func paymentAuthorizationViewControllerWillAuthorizePayment(PKPaymentAuthorizationViewController)

Tells the delegate that the user is authorizing the payment request.

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

