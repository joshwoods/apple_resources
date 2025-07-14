

- Apple Pay on the Web
- ApplePayRequest
-  requiredShippingContactFields 

Instance Property

# requiredShippingContactFields

The fields of shipping information the user must provide to fulfill the order.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
sequence  requiredShippingContactFields;
```

## Mentioned in 

Apple Pay on the Web Version 6 Release Notes

## Discussion

Use requiredShippingContactFields to request the user’s address and other contact information that you require to fulfill the order.

You receive the customer’s name when you request `postalAddress`. If you don’t need the customer’s address, you can request the name contact field directly.

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

The source of the information may be the user’s My Card in Contacts or in Wallet. The user can also enter the information into the payment sheet, either directly or through Contacts.

The requiredShippingContactFields for ApplePayRequest is available in Apple Pay version 6.

## See Also

### Requesting billing and shipping contact information

requiredBillingContactFields

The fields of billing information the user must provide to process the transaction.

