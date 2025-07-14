

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationControllerDelegate
-  paymentAuthorizationController(\_:didSelectShippingMethod:completion:) Deprecated

Instance Method

# paymentAuthorizationController(\_:didSelectShippingMethod:completion:)

Tells the delegate that the user selected a shipping method.

iOS 10.0–11.0DeprecatediPadOS 10.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 11.0+visionOS 1.0–1.0DeprecatedwatchOS 3.0–4.0Deprecated

**iOS, iPadOS, Mac Catalyst, macOS, visionOS, watchOS**

``` source
optional func paymentAuthorizationController(
    _ controller: PKPaymentAuthorizationController,
    didSelectShippingMethod shippingMethod: PKShippingMethod,
    completion: @escaping (PKPaymentAuthorizationStatus, [PKPaymentSummaryItem]) -> Void
)
```

**Mac Catalyst, macOS, visionOS**

``` source
optional func paymentAuthorizationController(
    _ controller: PKPaymentAuthorizationController,
    didSelectShippingMethod shippingMethod: PKShippingMethod
) async -> (PKPaymentAuthorizationStatus, [PKPaymentSummaryItem])
```

Deprecated

Use paymentAuthorizationController(_:didSelectShippingMethod:handler:) instead.

## Parameters 

`controller`  

The payment authorization controller.

`shippingMethod`  

The selected shipping method. This parameter contains one of the shipping methods included in the payment request.

`completion`  

The completion block to call with the updated payment summary items.

This block takes the following parameters:

`status`  
The authorization status for the payment. For values, see paymentAuthorizationControllerDidFinish(_:).

`summaryItems`  
An array of PKPaymentSummaryItem objects that replaces the summary items for the current payment request.

## Discussion

Use this method to update shipping costs based on the shipping address selected by the user, as previously passed to the delegate in the paymentAuthorizationController(_:didSelectShippingContact:completion:) method. If no address has been selected, use the prepopulated address on the payment request.

When this method is called, you create a new array of PKPaymentSummaryItem objects that represent the updated cost including shipping. For more information on creating summary items, see the PKPaymentRequest class’s paymentSummaryItems property.

Note

The delegate receives no further callbacks except paymentAuthorizationControllerDidFinish(_:) until it has invoked the completion block.

## See Also

### Handling shipping information

func paymentAuthorizationController(PKPaymentAuthorizationController, didSelectShippingContact: PKContact, handler: (PKPaymentRequestShippingContactUpdate) -> Void)

Tells the delegate that the user selected a shipping address.

func paymentAuthorizationController(PKPaymentAuthorizationController, didSelectShippingContact: PKContact, completion: (PKPaymentAuthorizationStatus, [PKShippingMethod], [PKPaymentSummaryItem]) -> Void)

Tells the delegate that the user selected a shipping address.

Deprecated

func paymentAuthorizationController(PKPaymentAuthorizationController, didSelectShippingMethod: PKShippingMethod, handler: (PKPaymentRequestShippingMethodUpdate) -> Void)

Tells the delegate that the user selected a shipping method.

