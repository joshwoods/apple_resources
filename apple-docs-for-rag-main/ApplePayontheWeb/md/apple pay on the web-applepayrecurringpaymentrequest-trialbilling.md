

- Apple Pay on the Web
- ApplePayRecurringPaymentRequest
-  trialBilling 

Instance Property

# trialBilling

The trial billing cycle for the recurring payment.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
ApplePayLineItem trialBilling;
```

## Discussion

The trial billing cycle is optional; use it if the recurring payment has a trial period.

Note

Set the paymentTiming property of the line item to `"recurring"` to avoid an error.

## See Also

### Setting the payment summary items

regularBilling

The regular billing cycle for the recurring payment, including start and end dates, an interval, and an interval count.

ApplePayLineItem

A line item in a payment request—for example, total, tax, discount, or grand total.

