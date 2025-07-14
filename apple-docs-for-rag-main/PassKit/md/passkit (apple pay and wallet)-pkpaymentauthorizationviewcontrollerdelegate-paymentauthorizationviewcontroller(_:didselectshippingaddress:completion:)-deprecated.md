

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationViewControllerDelegate
-  paymentAuthorizationViewController(\_:didSelectShippingAddress:completion:) Deprecated

Instance Method

# paymentAuthorizationViewController(\_:didSelectShippingAddress:completion:)

Tells the delegate that the user selected a shipping address.

iOS 8.0–9.0DeprecatediPadOS 8.0–9.0Deprecated

``` source
optional func paymentAuthorizationViewController(
    _ controller: PKPaymentAuthorizationViewController,
    didSelectShippingAddress address: ABRecord,
    completion: @escaping (PKPaymentAuthorizationStatus, [PKShippingMethod], [PKPaymentSummaryItem]) -> Void
)
```

Deprecated

This method is deprecated. Use paymentAuthorizationViewController(_:didSelectShippingContact:completion:) instead.

## Parameters 

`controller`  

The payment authorization view controller.

`address`  

An address book record representing the selected shipping method.

`completion`  

The completion block to be called with updated shipping information.

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

