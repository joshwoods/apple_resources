

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationControllerDelegate
-  paymentAuthorizationController(\_:didSelectShippingContact:handler:) 

Instance Method

# paymentAuthorizationController(\_:didSelectShippingContact:handler:)

Tells the delegate that the user selected a shipping address.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
@MainActor
optional func paymentAuthorizationController(
    _ controller: PKPaymentAuthorizationController,
    didSelectShippingContact contact: PKContact,
    handler completion: @escaping (PKPaymentRequestShippingContactUpdate) -> Void
)
```

``` source
@MainActor
optional func paymentAuthorizationController(
    _ controller: PKPaymentAuthorizationController,
    didSelectShippingContact contact: PKContact
) async -> PKPaymentRequestShippingContactUpdate
```

## Parameters 

`controller`  

The payment authorization controller.

`contact`  

A contact object that represents the new shipping address. To maintain privacy, the shipping information is anonymized. For example, in the United States it only includes the city, state, and zip code. This provides enough information to calculate shipping costs, without revealing sensitive information until the user actually approves the purchase.

`completion`  

The completion handler to call with the updated payment summary items and shipping methods.

## Discussion

Use this method to update the available shipping methods by creating a new array of valid PKShippingMethod objects for the specified address. You also create an array of PKPaymentSummaryItem objects that represent the updated cost if the user selects a valid shipping method. For more information on updating these values, see the PKPaymentRequest class’s shippingMethods and paymentSummaryItems properties.

## See Also

### Handling shipping information

func paymentAuthorizationController(PKPaymentAuthorizationController, didSelectShippingContact: PKContact, completion: (PKPaymentAuthorizationStatus, [PKShippingMethod], [PKPaymentSummaryItem]) -> Void)

Tells the delegate that the user selected a shipping address.

Deprecated

func paymentAuthorizationController(PKPaymentAuthorizationController, didSelectShippingMethod: PKShippingMethod, handler: (PKPaymentRequestShippingMethodUpdate) -> Void)

Tells the delegate that the user selected a shipping method.

func paymentAuthorizationController(PKPaymentAuthorizationController, didSelectShippingMethod: PKShippingMethod, completion: (PKPaymentAuthorizationStatus, [PKPaymentSummaryItem]) -> Void)

Tells the delegate that the user selected a shipping method.

Deprecated

