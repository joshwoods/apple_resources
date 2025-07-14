

- Apple Pay on the Web
- ApplePayPaymentRequest
-  shippingContactEditingMode 

Instance Property

# shippingContactEditingMode

A value that indicates whether the shipping mode prevents the user from editing the shipping address.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
ApplePayShippingContactEditingMode shippingContactEditingMode;
```

## Mentioned in 

Apple Pay on the Web Version 12 Release Notes

## Discussion

Set the value to `storePickup` for an in-store or other pickup to prevent the user from editing the shipping address.

Add `postalAddress` to `requiredShippingContactFields` to display the pickup address. Set the `shippingContact` to the pickup address.

```
let applePayPaymentRequest = {
    // Set the shipping type.
    shippingType: "storePickup",

    // Set the required shipping contact fields to display the pickup address.
    requiredShippingContactFields: [
        "postalAddress"
    ],

    // Set the shipping contact to the pickup location.
    shippingContact: {
        addressLines: ["123 Any Street"],
        locality: "Any Town",
        administrativeArea: "CA",
        postalCode: "95014",
        countryCode: "US",
        familyName: "COMPANY, INC."
    },

    // Set the shipping contact information to read-only.
    shippingContactEditingMode: "storePickup",

    countryCode: "US",
    currencyCode: "USD",
    merchantCapabilities: ["supports3DS"],
    supportedNetworks: ["visa", "masterCard"],
    total: { label: "COMPANY, INC.", amount: "10.00" }
};
```

Note

Determine whether to disable editing of the shipping contact field before displaying the payment sheet. Switching from a noneditable to an editable shipping contact field requires the user to start the payment process over again.

## See Also

### Requesting billing and shipping contact information

requiredBillingContactFields

The fields of billing information the user must provide to process the transaction.

requiredShippingContactFields

The fields of shipping information the user must provide to fulfill the order.

ApplePayContactField

Field names for requesting contact information in a payment request.

ApplePayShippingContactEditingMode

Values that indicate whether the shipping mode prevents the user from editing fields of the shipping address.

