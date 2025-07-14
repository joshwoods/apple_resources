

- Apple Pay on the Web
- ApplePayAutomaticReloadPaymentRequest
-  automaticReloadBilling 

Instance Property

# automaticReloadBilling

A line item that contains the reload amount and balance threshold for the automatic reload payment.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
required ApplePayLineItem automaticReloadBilling;
```

## Discussion

This line item describes an automatic reload payment.

Set the automaticReloadPaymentThresholdAmount to indicate the balance that the account drops below before the merchant applies the automatic reload amount. Set the amount object to specify the reload amount.

Note

Set the paymentTiming property of the line item to `"automaticReload"` to avoid an error.

## See Also

### Setting the payment summary items

ApplePayLineItem

A line item in a payment request—for example, total, tax, discount, or grand total.

