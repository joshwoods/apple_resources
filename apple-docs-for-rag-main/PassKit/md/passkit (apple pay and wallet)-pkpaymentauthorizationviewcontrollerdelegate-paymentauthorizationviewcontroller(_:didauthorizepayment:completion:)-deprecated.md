

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationViewControllerDelegate
-  paymentAuthorizationViewController(\_:didAuthorizePayment:completion:) Deprecated

Instance Method

# paymentAuthorizationViewController(\_:didAuthorizePayment:completion:)

Tells the delegate that the user authorized the payment request, and asks for a result.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 11.0+visionOS 1.0–1.0Deprecated

**iOS, iPadOS, Mac Catalyst, macOS, visionOS**

``` source
optional func paymentAuthorizationViewController(
    _ controller: PKPaymentAuthorizationViewController,
    didAuthorizePayment payment: PKPayment,
    completion: @escaping (PKPaymentAuthorizationStatus) -> Void
)
```

**Mac Catalyst, macOS, visionOS**

``` source
optional func paymentAuthorizationViewController(
    _ controller: PKPaymentAuthorizationViewController,
    didAuthorizePayment payment: PKPayment
) async -> PKPaymentAuthorizationStatus
```

Deprecated

Use paymentAuthorizationViewController(_:didAuthorizePayment:handler:) instead.

## Parameters 

`controller`  

The payment authorization view controller.

`payment`  

The authorized payment. This object contains the payment token you need to submit to your payment processor, as well as the billing and shipping information required by the payment request.

`completion`  

The completion block to call with the result of authorizing the payment.

This block takes the following parameters:

`status`  
The authorization status for the payment. For values, see PKPaymentAuthorizationStatus.

## Discussion

This method is called after the payment request is authorized. You submit the payment information to your payment processor to authorize the transaction, and then call the completion block.

## See Also

### Handling user’s payment authorization

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didRequestMerchantSessionUpdate: (PKPaymentRequestMerchantSessionUpdate) -> Void)

Requests an object that validates the identity of a merchant for a payment request.

func paymentAuthorizationViewControllerWillAuthorizePayment(PKPaymentAuthorizationViewController)

Tells the delegate that the user is authorizing the payment request.

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didAuthorizePayment: PKPayment, handler: (PKPaymentAuthorizationResult) -> Void)

Tells the delegate that the user authorized the payment request, and asks for a result.

func paymentAuthorizationViewControllerDidFinish(PKPaymentAuthorizationViewController)

Tells the delegate that payment authorization finished.

**Required**

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didSelect: PKPaymentMethod, handler: (PKPaymentRequestPaymentMethodUpdate) -> Void)

Tells the delegate that the user changed the payment method, and asks for an updated payment request.

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didSelect: PKPaymentMethod, completion: ([PKPaymentSummaryItem]) -> Void)

Tells the delegate that the user changed the payment method, and asks for an updated payment request.

Deprecated

