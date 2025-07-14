

- Apple Pay on the Web
- ApplePayPaymentRequest
-  requiredBillingContactFields 

Instance Property

# requiredBillingContactFields

The fields of billing information the user must provide to process the transaction.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
sequence  requiredBillingContactFields;
```

## Discussion

Use `requiredBillingContactFields` to request the user’s billing address that is associated with their payment method. The field you can request for a billing contact is shown in the following sample code:

```
"requiredBillingContactFields": [
    "postalAddress"
]
```

You will receive the postal address as well as the user’s name after the user authorizes the transaction.

The source of the information may be the user’s Me contact card, the back of credit card in Wallet, or may be entered by the user directly into the payment sheet.

## See Also

### Requesting billing and shipping contact information

requiredShippingContactFields

The fields of shipping information the user must provide to fulfill the order.

shippingContactEditingMode

A value that indicates whether the shipping mode prevents the user from editing the shipping address.

ApplePayContactField

Field names for requesting contact information in a payment request.

ApplePayShippingContactEditingMode

Values that indicate whether the shipping mode prevents the user from editing fields of the shipping address.

