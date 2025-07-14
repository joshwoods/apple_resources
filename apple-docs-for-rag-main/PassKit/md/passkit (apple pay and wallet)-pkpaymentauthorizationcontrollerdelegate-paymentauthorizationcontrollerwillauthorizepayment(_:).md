

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationControllerDelegate
-  paymentAuthorizationControllerWillAuthorizePayment(\_:) 

Instance Method

# paymentAuthorizationControllerWillAuthorizePayment(\_:)

Tells the delegate that the user is authorizing the payment request.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
@MainActor
optional func paymentAuthorizationControllerWillAuthorizePayment(_ controller: PKPaymentAuthorizationController)
```

## Parameters 

`controller`  

The payment authorization controller.

## Discussion

This method is called before the payment request is authorized but after the user has authenticated by using either a passcode, Touch ID, or Face ID.

## See Also

### Handling user’s payment authorization

func paymentAuthorizationController(PKPaymentAuthorizationController, didRequestMerchantSessionUpdate: (PKPaymentRequestMerchantSessionUpdate) -> Void)

Requests an object that validates the identity of a merchant for a payment request.

func paymentAuthorizationController(PKPaymentAuthorizationController, didAuthorizePayment: PKPayment, handler: (PKPaymentAuthorizationResult) -> Void)

Tells the delegate that the user authorized the payment request, and asks for a result.

func paymentAuthorizationController(PKPaymentAuthorizationController, didAuthorizePayment: PKPayment, completion: (PKPaymentAuthorizationStatus) -> Void)

Tells the delegate that the user authorized the payment request, and asks for a result.

Deprecated

func paymentAuthorizationControllerDidFinish(PKPaymentAuthorizationController)

Tells the delegate that payment authorization has completed.

**Required**

