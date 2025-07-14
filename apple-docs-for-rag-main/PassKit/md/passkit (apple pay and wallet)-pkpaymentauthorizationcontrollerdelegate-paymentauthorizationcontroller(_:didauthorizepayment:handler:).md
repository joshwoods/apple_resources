

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationControllerDelegate
-  paymentAuthorizationController(\_:didAuthorizePayment:handler:) 

Instance Method

# paymentAuthorizationController(\_:didAuthorizePayment:handler:)

Tells the delegate that the user authorized the payment request, and asks for a result.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
@MainActor
optional func paymentAuthorizationController(
    _ controller: PKPaymentAuthorizationController,
    didAuthorizePayment payment: PKPayment,
    handler completion: @escaping (PKPaymentAuthorizationResult) -> Void
)
```

``` source
@MainActor
optional func paymentAuthorizationController(
    _ controller: PKPaymentAuthorizationController,
    didAuthorizePayment payment: PKPayment
) async -> PKPaymentAuthorizationResult
```

## Parameters 

`controller`  

The payment authorization controller.

`payment`  

The authorized payment. This object contains the payment token you need to submit to your payment processor, as well as the billing and shipping information required by the payment request.

`completion`  

The completion handler to call with the result of authorizing the payment.

## Discussion

The system calls this method after the payment request is authorized. You submit the payment information to your payment processor to authorize the transaction, and then call the handler.

## See Also

### Handling user’s payment authorization

func paymentAuthorizationController(PKPaymentAuthorizationController, didRequestMerchantSessionUpdate: (PKPaymentRequestMerchantSessionUpdate) -> Void)

Requests an object that validates the identity of a merchant for a payment request.

func paymentAuthorizationControllerWillAuthorizePayment(PKPaymentAuthorizationController)

Tells the delegate that the user is authorizing the payment request.

func paymentAuthorizationController(PKPaymentAuthorizationController, didAuthorizePayment: PKPayment, completion: (PKPaymentAuthorizationStatus) -> Void)

Tells the delegate that the user authorized the payment request, and asks for a result.

Deprecated

func paymentAuthorizationControllerDidFinish(PKPaymentAuthorizationController)

Tells the delegate that payment authorization has completed.

**Required**

