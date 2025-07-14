

- Apple Pay on the Web
- ApplePayRequest
-  requiredBillingContactFields 

Instance Property

# requiredBillingContactFields

The fields of billing information the user must provide to process the transaction.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
sequence  requiredBillingContactFields;
```

## Discussion

Use requiredBillingContactFields to request the user’s billing address that’s associated with their payment method, as shown in the following listing.

```
"requiredBillingContactFields": [
    "postalAddress"
]
```

You’ll receive the postal address as well as the user’s name after the user authorizes the transaction.

The source of the information may be the user’s “My card” in Contacts, Wallet settings, or may be entered by the user into the payment sheet, either directly or through Contacts.

## See Also

### Requesting billing and shipping contact information

requiredShippingContactFields

The fields of shipping information the user must provide to fulfill the order.

