

- Apple Pay on the Web
- ApplePayPaymentRequest
-  requiredShippingContactFields 

Instance Property

# requiredShippingContactFields

The fields of shipping information the user must provide to fulfill the order.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
sequence  requiredShippingContactFields;
```

## Discussion

Use `requiredShippingContactFields` to request the user’s address and other contact information that you require to fulfill the order.

You will receive the customer’s name when you request `postalAddress`. If you don’t need the customer’s address, you can request the `name` contact field directly.

The following listing is an example of requesting fields for a shipping contact:

```
"requiredShippingContactFields": [
    "postalAddress",
    "name",
    "phoneticName",
    "phone",
    "email"
]
```

The source of the information may be the user’s “My card” in Contacts, Wallet settings, or may be entered into the payment sheet by the user, either directly or through Contacts.

## See Also

### Requesting billing and shipping contact information

requiredBillingContactFields

The fields of billing information the user must provide to process the transaction.

shippingContactEditingMode

A value that indicates whether the shipping mode prevents the user from editing the shipping address.

ApplePayContactField

Field names for requesting contact information in a payment request.

ApplePayShippingContactEditingMode

Values that indicate whether the shipping mode prevents the user from editing fields of the shipping address.

