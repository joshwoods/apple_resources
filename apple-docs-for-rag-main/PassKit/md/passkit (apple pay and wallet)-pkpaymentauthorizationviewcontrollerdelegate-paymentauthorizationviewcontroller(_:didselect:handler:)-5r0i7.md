

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationViewControllerDelegate
-  paymentAuthorizationViewController(\_:didSelect:handler:) 

Instance Method

# paymentAuthorizationViewController(\_:didSelect:handler:)

Tells the delegate that the user selected a shipping method, and asks for an updated payment request.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+

``` source
optional func paymentAuthorizationViewController(
    _ controller: PKPaymentAuthorizationViewController,
    didSelect shippingMethod: PKShippingMethod,
    handler completion: @escaping (PKPaymentRequestShippingMethodUpdate) -> Void
)
```

``` source
optional func paymentAuthorizationViewController(
    _ controller: PKPaymentAuthorizationViewController,
    didSelect shippingMethod: PKShippingMethod
) async -> PKPaymentRequestShippingMethodUpdate
```

## Parameters 

`controller`  

The payment authorization view controller.

`shippingMethod`  

The selected shipping method. This parameter contains one of the shipping methods specified in the payment request.

`completion`  

The completion handler to call with the updated payment summary items.

## Discussion

Use this method to update shipping costs based on the shipping address the user selected in a call to paymentAuthorizationViewController(_:didSelectShippingContact:handler:). If the user didn’t select an address, use the prepopulated address of the payment request.

When the system calls this method, you create a new array of PKPaymentSummaryItem objects that represent the updated cost including shipping. For more information on creating summary items, see the PKPaymentRequest class’s paymentSummaryItems property.

## See Also

### Handling shipping information

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didSelectShippingContact: PKContact, handler: (PKPaymentRequestShippingContactUpdate) -> Void)

Tells the delegate that the user selected a shipping address, and asks for an updated payment request.

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didSelectShippingContact: PKContact, completion: (PKPaymentAuthorizationStatus, [PKShippingMethod], [PKPaymentSummaryItem]) -> Void)

Tells the delegate that the user selected a shipping address, and asks for an updated payment request.

Deprecated

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didSelect: PKShippingMethod, completion: (PKPaymentAuthorizationStatus, [PKPaymentSummaryItem]) -> Void)

Tells the delegate that the user selected a shipping method, and asks for an updated payment request.

Deprecated

