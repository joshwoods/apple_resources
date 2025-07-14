

- Apple Pay on the Web
- ApplePayRecurringPaymentRequest
-  regularBilling 

Instance Property

# regularBilling

The regular billing cycle for the recurring payment, including start and end dates, an interval, and an interval count.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
required ApplePayLineItem regularBilling;
```

## Discussion

This line item applies to a regular billing cycle for a recurring payment.

Note

Set the paymentTiming property of the line item to `"recurring"` to avoid an error.

## See Also

### Setting the payment summary items

trialBilling

The trial billing cycle for the recurring payment.

ApplePayLineItem

A line item in a payment request—for example, total, tax, discount, or grand total.

