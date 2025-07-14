

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationControllerDelegate
-  paymentAuthorizationController(\_:didSelectShippingMethod:handler:) 

Instance Method

# paymentAuthorizationController(\_:didSelectShippingMethod:handler:)

Tells the delegate that the user selected a shipping method.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
@MainActor
optional func paymentAuthorizationController(
    _ controller: PKPaymentAuthorizationController,
    didSelectShippingMethod shippingMethod: PKShippingMethod,
    handler completion: @escaping (PKPaymentRequestShippingMethodUpdate) -> Void
)
```

``` source
@MainActor
optional func paymentAuthorizationController(
    _ controller: PKPaymentAuthorizationController,
    didSelectShippingMethod shippingMethod: PKShippingMethod
) async -> PKPaymentRequestShippingMethodUpdate
```

## Parameters 

`controller`  

The payment authorization controller.

`shippingMethod`  

The selected shipping method. This parameter contains one of the shipping methods included in the payment request.

`completion`  

The completion handler to call with the updated payment summary items.

## Discussion

Use this method to update shipping costs based on the shipping address the user selected, as previously passed to the delegate in the paymentAuthorizationController(_:didSelectShippingContact:handler:) method. If the user didn’t select an address, use the prepopulated address on the payment request.

When the system calls this method, you create a new array of PKPaymentSummaryItem objects that represent the updated cost including shipping. For more information on creating summary items, see the PKPaymentRequest class’s paymentSummaryItems property.

## See Also

### Handling shipping information

func paymentAuthorizationController(PKPaymentAuthorizationController, didSelectShippingContact: PKContact, handler: (PKPaymentRequestShippingContactUpdate) -> Void)

Tells the delegate that the user selected a shipping address.

func paymentAuthorizationController(PKPaymentAuthorizationController, didSelectShippingContact: PKContact, completion: (PKPaymentAuthorizationStatus, [PKShippingMethod], [PKPaymentSummaryItem]) -> Void)

Tells the delegate that the user selected a shipping address.

Deprecated

func paymentAuthorizationController(PKPaymentAuthorizationController, didSelectShippingMethod: PKShippingMethod, completion: (PKPaymentAuthorizationStatus, [PKPaymentSummaryItem]) -> Void)

Tells the delegate that the user selected a shipping method.

Deprecated

