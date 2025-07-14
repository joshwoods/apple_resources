

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationViewControllerDelegate
-  paymentAuthorizationViewController(\_:didSelect:completion:) Deprecated

Instance Method

# paymentAuthorizationViewController(\_:didSelect:completion:)

Tells the delegate that the user changed the payment method, and asks for an updated payment request.

iOS 9.0–11.0DeprecatediPadOS 9.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 11.0+visionOS 1.0–1.0Deprecated

**iOS, iPadOS, Mac Catalyst, macOS, visionOS**

``` source
optional func paymentAuthorizationViewController(
    _ controller: PKPaymentAuthorizationViewController,
    didSelect paymentMethod: PKPaymentMethod,
    completion: @escaping ([PKPaymentSummaryItem]) -> Void
)
```

**Mac Catalyst, macOS, visionOS**

``` source
optional func paymentAuthorizationViewController(
    _ controller: PKPaymentAuthorizationViewController,
    didSelect paymentMethod: PKPaymentMethod
) async -> [PKPaymentSummaryItem]
```

Deprecated

Use paymentAuthorizationViewController(_:didSelect:handler:) instead.

## Parameters 

`controller`  

The payment authorization view controller.

`paymentMethod`  

The new payment method.

`completion`  

The completion block to call with the updated payment summary items.

This block takes the following parameters:

`summaryItems`  
An updated array of summary items that include any changes due to fees or credit card surcharges associated with the payment method.

## Discussion

This method is called when the user has selected a new payment card. Use this delegate callback to update the summary items in response to the card type changing (for example, applying credit card surcharges), and then call the callback with the updated summary items.

Note

The delegate receives no further callbacks except paymentAuthorizationViewControllerDidFinish(_:) until it has invoked the completion block.

## See Also

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

