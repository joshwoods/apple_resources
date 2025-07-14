

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationControllerDelegate
-  paymentAuthorizationControllerDidFinish(\_:) 

Instance Method

# paymentAuthorizationControllerDidFinish(\_:)

Tells the delegate that payment authorization has completed.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
@MainActor
func paymentAuthorizationControllerDidFinish(_ controller: PKPaymentAuthorizationController)
```

**Required**

## Parameters 

`controller`  

The payment authorization controller.

## Discussion

Use this method to dismiss the payment authorization controller and update any other app state.

When the user authorizes a payment request, this method is called after the user is shown the status from the paymentAuthorizationController(_:didAuthorizePayment:completion:) method’s completion block. When the user cancels without authorizing the payment request, only `paymentAuthorizationControllerDidFinish:` is called.

## See Also

### Handling user’s payment authorization

func paymentAuthorizationController(PKPaymentAuthorizationController, didRequestMerchantSessionUpdate: (PKPaymentRequestMerchantSessionUpdate) -> Void)

Requests an object that validates the identity of a merchant for a payment request.

func paymentAuthorizationControllerWillAuthorizePayment(PKPaymentAuthorizationController)

Tells the delegate that the user is authorizing the payment request.

func paymentAuthorizationController(PKPaymentAuthorizationController, didAuthorizePayment: PKPayment, handler: (PKPaymentAuthorizationResult) -> Void)

Tells the delegate that the user authorized the payment request, and asks for a result.

func paymentAuthorizationController(PKPaymentAuthorizationController, didAuthorizePayment: PKPayment, completion: (PKPaymentAuthorizationStatus) -> Void)

Tells the delegate that the user authorized the payment request, and asks for a result.

Deprecated

