

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationViewControllerDelegate
-  paymentAuthorizationViewController(\_:didSelectShippingContact:completion:) Deprecated

Instance Method

# paymentAuthorizationViewController(\_:didSelectShippingContact:completion:)

Tells the delegate that the user selected a shipping address, and asks for an updated payment request.

iOS 9.0–11.0DeprecatediPadOS 9.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 11.0+visionOS 1.0–1.0Deprecated

**iOS, iPadOS, Mac Catalyst, macOS, visionOS**

``` source
optional func paymentAuthorizationViewController(
    _ controller: PKPaymentAuthorizationViewController,
    didSelectShippingContact contact: PKContact,
    completion: @escaping (PKPaymentAuthorizationStatus, [PKShippingMethod], [PKPaymentSummaryItem]) -> Void
)
```

**Mac Catalyst, macOS, visionOS**

``` source
optional func paymentAuthorizationViewController(
    _ controller: PKPaymentAuthorizationViewController,
    didSelectShippingContact contact: PKContact
) async -> (PKPaymentAuthorizationStatus, [PKShippingMethod], [PKPaymentSummaryItem])
```

Deprecated

Use paymentAuthorizationViewController(_:didSelectShippingContact:handler:) instead.

## Parameters 

`controller`  

The payment authorization view controller.

`contact`  

A contact object representing the new shipping address. To maintain privacy, the shipping information is anonymized. For example, in the United States it only includes the city, state, and zip code. This provides enough information to calculate shipping costs, without revealing sensitive information until the user actually approves the purchase.

`completion`  

The completion block to call with the updated payment summary items and shipping methods.

This block takes the following parameters:

`status`  
The authorization status for the payment. For values, see PKPaymentAuthorizationViewControllerDelegate.

`shippingMethods`  
An array of PKShippingMethod objects that replaces the shipping methods for the current payment request.

`summaryItems`  
An array of PKPaymentSummaryItem objects that replaces the summary items for the current payment request.

## Discussion

Use this method to update the available shipping methods and, if a shipping method has been selected, the current shipping cost.

When this method is called, you create a new array of valid PKShippingMethod objects for the specified address. You also create an array of PKPaymentSummaryItem objects that represent the updated cost. The summary items should include the shipping cost if a valid shipping method has been selected. For more information on updating these values, see the PKPaymentRequest class’s shippingMethods and paymentSummaryItems properties.

## See Also

### Handling shipping information

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didSelectShippingContact: PKContact, handler: (PKPaymentRequestShippingContactUpdate) -> Void)

Tells the delegate that the user selected a shipping address, and asks for an updated payment request.

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didSelect: PKShippingMethod, handler: (PKPaymentRequestShippingMethodUpdate) -> Void)

Tells the delegate that the user selected a shipping method, and asks for an updated payment request.

func paymentAuthorizationViewController(PKPaymentAuthorizationViewController, didSelect: PKShippingMethod, completion: (PKPaymentAuthorizationStatus, [PKPaymentSummaryItem]) -> Void)

Tells the delegate that the user selected a shipping method, and asks for an updated payment request.

Deprecated

