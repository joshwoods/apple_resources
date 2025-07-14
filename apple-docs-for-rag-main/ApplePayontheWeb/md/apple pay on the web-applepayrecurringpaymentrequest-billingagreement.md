

- Apple Pay on the Web
- ApplePayRecurringPaymentRequest
-  billingAgreement 

Instance Property

# billingAgreement

A localized billing agreement that the payment sheet displays to the user before the user authorizes the payment.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
DOMString billingAgreement;
```

## Discussion

The merchant may provide an optional, localized billingAgreement string. The maximum length of the billingAgreement string is 500 characters.

You may use this string to include information about the recurring payment amount, interval, or other payment conditions, for example, or information on how the user can cancel payments. This string isn’t intended to replace any payment terms that you provide outside of the Apple Pay payment sheet.

Important

You’re responsible to ensure that your use of this framework, including your billing agreement, is compliant with applicable legal requirements.

The Apple Pay payment sheet displays the text of the billingAgreement string; however, long billingAgreement strings that don’t fit on the payment sheet screen appear truncated with an ellipsis. Users can select the Billing Details on the payment sheet to read the full text of the billingAgreement string, up to the maximum 500 characters.

## See Also

### Describing the recurring payment

paymentDescription

A description of the recurring payment that Apple Pay displays to the user in the payment sheet.

