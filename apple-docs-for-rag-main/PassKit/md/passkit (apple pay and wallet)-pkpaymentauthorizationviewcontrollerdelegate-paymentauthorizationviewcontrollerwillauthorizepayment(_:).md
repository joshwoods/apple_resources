

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationViewControllerDelegate
-  paymentAuthorizationViewControllerWillAuthorizePayment(\_:) 

Instance Method

# paymentAuthorizationViewControllerWillAuthorizePayment(\_:)

Tells the delegate that the user is authorizing the payment request.

iOS 8.3+iPadOS 8.3+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+

``` source
optional func paymentAuthorizationViewControllerWillAuthorizePayment(_ controller: PKPaymentAuthorizationViewController)
```

## Parameters 

`controller`  

The payment authorization view controller.

## Discussion

This method is called before the payment request is authorized but after the user has authenticated by using either a passcode, Touch ID, or Face ID.

## See Also

### Related Documentation

Wallet Developer Guide

### Handling user’s payment authorization

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didRequestMerchantSessionUpdate: (PKPaymentRequestMerchantSessionUpdate) -> Void)

Requests an object that validates the identity of a merchant for a payment request.

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

