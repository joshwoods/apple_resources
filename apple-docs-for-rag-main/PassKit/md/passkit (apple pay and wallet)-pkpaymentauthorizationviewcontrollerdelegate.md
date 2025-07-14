

- PassKit (Apple Pay and Wallet)
-  PKPaymentAuthorizationViewControllerDelegate 

Protocol

# PKPaymentAuthorizationViewControllerDelegate

Methods that let you respond to user interactions with your payment authorization view controller.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
protocol PKPaymentAuthorizationViewControllerDelegate : NSObjectProtocol
```

## Overview

The PKPaymentAuthorizationViewControllerDelegate protocol is implemented by the payment authorization view controller’s delegate. You implement this protocol to respond to user interaction with that view controller.

The payment authorization view controller automatically waits for its delegate to finish responding to one method before it calls other delegate methods. You indicate that the delegate is finished with the current method by calling that method’s completion block. This action tells the pay authorization view controller to proceed with the next step in the authorization process.

There is one exception to this step-by-step procedure: The pay authorization view controller calls the paymentAuthorizationViewControllerDidFinish(_:) method as soon as the user cancels a payment without authorizing a payment request, or when a payment is canceled after timing out. The controller can call this method at any time.

## Topics

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

func paymentAuthorizationViewControllerDidFinish(PKPaymentAuthorizationViewController)

Tells the delegate that payment authorization finished.

**Required**

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didSelect: PKPaymentMethod, handler: (PKPaymentRequestPaymentMethodUpdate) -> Void)

Tells the delegate that the user changed the payment method, and asks for an updated payment request.

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didSelect: PKPaymentMethod, completion: ([PKPaymentSummaryItem]) -> Void)

Tells the delegate that the user changed the payment method, and asks for an updated payment request.

Deprecated

### Handling coupons

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didChangeCouponCode: String, handler: (PKPaymentRequestCouponCodeUpdate) -> Void)

Tells the delegate that the user entered or updated a coupon code.

### Handling shipping information

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didSelectShippingContact: PKContact, handler: (PKPaymentRequestShippingContactUpdate) -> Void)

Tells the delegate that the user selected a shipping address, and asks for an updated payment request.

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didSelectShippingContact: PKContact, completion: (PKPaymentAuthorizationStatus, [PKShippingMethod], [PKPaymentSummaryItem]) -> Void)

Tells the delegate that the user selected a shipping address, and asks for an updated payment request.

Deprecated

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didSelect: PKShippingMethod, handler: (PKPaymentRequestShippingMethodUpdate) -> Void)

Tells the delegate that the user selected a shipping method, and asks for an updated payment request.

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didSelect: PKShippingMethod, completion: (PKPaymentAuthorizationStatus, [PKPaymentSummaryItem]) -> Void)

Tells the delegate that the user selected a shipping method, and asks for an updated payment request.

Deprecated

### Deprecated

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didSelectShippingAddress: ABRecord, completion: (PKPaymentAuthorizationStatus, [PKShippingMethod], [PKPaymentSummaryItem]) -> Void)

Tells the delegate that the user selected a shipping address.

Deprecated

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Handling user interactions

var delegate: (any PKPaymentAuthorizationViewControllerDelegate)?

The view controller’s delegate.

