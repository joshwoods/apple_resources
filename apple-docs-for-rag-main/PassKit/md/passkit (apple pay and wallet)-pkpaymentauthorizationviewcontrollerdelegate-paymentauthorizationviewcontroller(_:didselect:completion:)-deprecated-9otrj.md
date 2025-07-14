

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationViewControllerDelegate
-  paymentAuthorizationViewController(\_:didSelect:completion:) Deprecated

Instance Method

# paymentAuthorizationViewController(\_:didSelect:completion:)

Tells the delegate that the user selected a shipping method, and asks for an updated payment request.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 11.0+visionOS 1.0–1.0Deprecated

**iOS, iPadOS, Mac Catalyst, macOS, visionOS**

``` source
optional func paymentAuthorizationViewController(
    _ controller: PKPaymentAuthorizationViewController,
    didSelect shippingMethod: PKShippingMethod,
    completion: @escaping (PKPaymentAuthorizationStatus, [PKPaymentSummaryItem]) -> Void
)
```

**Mac Catalyst, macOS, visionOS**

``` source
optional func paymentAuthorizationViewController(
    _ controller: PKPaymentAuthorizationViewController,
    didSelect shippingMethod: PKShippingMethod
) async -> (PKPaymentAuthorizationStatus, [PKPaymentSummaryItem])
```

Deprecated

Use paymentAuthorizationViewController(_:didSelect:handler:) instead.

## Parameters 

`controller`  

The payment authorization view controller.

`shippingMethod`  

The selected shipping method. This parameter contains one of the shipping methods included in the payment request.

`completion`  

The completion block to call with the updated payment summary items.

This block takes the following parameters:

`status`  
The authorization status for the payment. For values, see PKPaymentAuthorizationStatus.

`summaryItems`  
An array of PKPaymentSummaryItem objects that replaces the summary items for the current payment request.

## Discussion

Use this method to update shipping costs based on the shipping address selected by the user, as previously passed to the delegate in the PKPaymentAuthorizationViewControllerDelegate method. If no address has been selected, use the prepopulated address on the payment request.

When this method is called, you create a new array of PKPaymentSummaryItem objects that represent the updated cost including shipping. For more information on creating summary items, see the PKPaymentRequest class’s paymentSummaryItems property.

## See Also

### Handling shipping information

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didSelectShippingContact: PKContact, handler: (PKPaymentRequestShippingContactUpdate) -> Void)

Tells the delegate that the user selected a shipping address, and asks for an updated payment request.

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didSelectShippingContact: PKContact, completion: (PKPaymentAuthorizationStatus, [PKShippingMethod], [PKPaymentSummaryItem]) -> Void)

Tells the delegate that the user selected a shipping address, and asks for an updated payment request.

Deprecated

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didSelect: PKShippingMethod, handler: (PKPaymentRequestShippingMethodUpdate) -> Void)

Tells the delegate that the user selected a shipping method, and asks for an updated payment request.

