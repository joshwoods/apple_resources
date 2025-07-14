

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationControllerDelegate
-  paymentAuthorizationController(\_:didRequestMerchantSessionUpdate:) 

Instance Method

# paymentAuthorizationController(\_:didRequestMerchantSessionUpdate:)

Requests an object that validates the identity of a merchant for a payment request.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+watchOS 7.0+

``` source
@MainActor
optional func paymentAuthorizationController(
    _ controller: PKPaymentAuthorizationController,
    didRequestMerchantSessionUpdate handler: @escaping (PKPaymentRequestMerchantSessionUpdate) -> Void
)
```

``` source
@MainActor
optional func paymentAuthorizationControllerDidRequestMerchantSessionUpdate(controller: PKPaymentAuthorizationController) async -> PKPaymentRequestMerchantSessionUpdate
```

## Parameters 

`controller`  

The payment authorization controller.

`handler`  

The completion handler to call with the updated merchant session.

## See Also

### Handling user’s payment authorization

func paymentAuthorizationControllerWillAuthorizePayment(PKPaymentAuthorizationController)

Tells the delegate that the user is authorizing the payment request.

func paymentAuthorizationController(PKPaymentAuthorizationController, didAuthorizePayment: PKPayment, handler: (PKPaymentAuthorizationResult) -> Void)

Tells the delegate that the user authorized the payment request, and asks for a result.

func paymentAuthorizationController(PKPaymentAuthorizationController, didAuthorizePayment: PKPayment, completion: (PKPaymentAuthorizationStatus) -> Void)

Tells the delegate that the user authorized the payment request, and asks for a result.

Deprecated

func paymentAuthorizationControllerDidFinish(PKPaymentAuthorizationController)

Tells the delegate that payment authorization has completed.

**Required**

