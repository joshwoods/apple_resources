

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationViewControllerDelegate
-  paymentAuthorizationViewController(\_:didSelectShippingContact:handler:) 

Instance Method

# paymentAuthorizationViewController(\_:didSelectShippingContact:handler:)

Tells the delegate that the user selected a shipping address, and asks for an updated payment request.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+

``` source
optional func paymentAuthorizationViewController(
    _ controller: PKPaymentAuthorizationViewController,
    didSelectShippingContact contact: PKContact,
    handler completion: @escaping (PKPaymentRequestShippingContactUpdate) -> Void
)
```

``` source
optional func paymentAuthorizationViewController(
    _ controller: PKPaymentAuthorizationViewController,
    didSelectShippingContact contact: PKContact
) async -> PKPaymentRequestShippingContactUpdate
```

## Parameters 

`controller`  

The payment authorization view controller.

`contact`  

A contact object that represents the new shipping address. To maintain privacy, the shipping information is anonymized. For example, in the United States it only includes the city, state, and zip code. This information provides enough detail to calculate shipping costs, without revealing sensitive information until the user actually approves the purchase.

`completion`  

The completion handler to call with the updated payment summary items and shipping methods.

## Discussion

Use this method to update the available shipping methods by creating a new array of valid PKShippingMethod objects for the specified address. You also create an array of PKPaymentSummaryItem objects that represent the updated cost if the user selected a valid shipping method. For more information on updating these values, see the PKPaymentRequest class’s shippingMethods and paymentSummaryItems properties.

## See Also

### Handling shipping information

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didSelectShippingContact: PKContact, completion: (PKPaymentAuthorizationStatus, [PKShippingMethod], [PKPaymentSummaryItem]) -> Void)

Tells the delegate that the user selected a shipping address, and asks for an updated payment request.

Deprecated

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didSelect: PKShippingMethod, handler: (PKPaymentRequestShippingMethodUpdate) -> Void)

Tells the delegate that the user selected a shipping method, and asks for an updated payment request.

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didSelect: PKShippingMethod, completion: (PKPaymentAuthorizationStatus, [PKPaymentSummaryItem]) -> Void)

Tells the delegate that the user selected a shipping method, and asks for an updated payment request.

Deprecated

