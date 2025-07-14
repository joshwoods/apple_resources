

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationControllerDelegate
-  paymentAuthorizationController(\_:didAuthorizePayment:completion:) Deprecated

Instance Method

# paymentAuthorizationController(\_:didAuthorizePayment:completion:)

Tells the delegate that the user authorized the payment request, and asks for a result.

iOS 10.0–11.0DeprecatediPadOS 10.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 11.0+visionOS 1.0–1.0DeprecatedwatchOS 3.0–4.0Deprecated

**iOS, iPadOS, Mac Catalyst, macOS, visionOS, watchOS**

``` source
optional func paymentAuthorizationController(
    _ controller: PKPaymentAuthorizationController,
    didAuthorizePayment payment: PKPayment,
    completion: @escaping (PKPaymentAuthorizationStatus) -> Void
)
```

**Mac Catalyst, macOS, visionOS**

``` source
optional func paymentAuthorizationController(
    _ controller: PKPaymentAuthorizationController,
    didAuthorizePayment payment: PKPayment
) async -> PKPaymentAuthorizationStatus
```

Deprecated

Use paymentAuthorizationController(_:didAuthorizePayment:handler:) instead.

## Parameters 

`controller`  

The payment authorization controller.

`payment`  

The authorized payment. This object contains the payment token you need to submit to your payment processor, as well as the billing and shipping information required by the payment request.

`completion`  

The completion block to call with the result of authorizing the payment.

This block takes the following parameters:

`status`  
The authorization status for the payment. For values, see paymentAuthorizationControllerDidFinish(_:).

## Discussion

This method is called after the payment request is authorized. You submit the payment information to your payment processor to authorize the transaction, and then call the completion block.

Note

The delegate receives no further callbacks except paymentAuthorizationControllerDidFinish(_:) until it has invoked the completion block.

## See Also

### Handling user’s payment authorization

func paymentAuthorizationController(PKPaymentAuthorizationController, didRequestMerchantSessionUpdate: (PKPaymentRequestMerchantSessionUpdate) -> Void)

Requests an object that validates the identity of a merchant for a payment request.

func paymentAuthorizationControllerWillAuthorizePayment(PKPaymentAuthorizationController)

Tells the delegate that the user is authorizing the payment request.

func paymentAuthorizationController(PKPaymentAuthorizationController, didAuthorizePayment: PKPayment, handler: (PKPaymentAuthorizationResult) -> Void)

Tells the delegate that the user authorized the payment request, and asks for a result.

func paymentAuthorizationControllerDidFinish(PKPaymentAuthorizationController)

Tells the delegate that payment authorization has completed.

**Required**

