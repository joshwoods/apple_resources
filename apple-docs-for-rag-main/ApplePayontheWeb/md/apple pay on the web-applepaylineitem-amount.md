

- Apple Pay on the Web
- ApplePayLineItem
-  amount 

Instance Property

# amount

A required value that’s the monetary amount of the line item.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
DOMString amount;
```

## Discussion

This number must follow the regular expression `-?[0-9]+(\.[0-9][0-9])?`. The amount is required and can’t be empty.

You specify the currency for the entire transaction including line items by setting the currencyCode property in ApplePayPaymentRequest.

If the payment request is for an automatic reload payment, the `amount` indicates the reload payment amount authorized when the account drops below the \`\`/ApplePayontheWeb/ApplePayLineItem/automaticReloadPaymentThresholdAmount\`\`\`.\`

## See Also

### Setting line item properties

label

A required value that’s a short, localized description of the line item.

type

A value that indicates whether the line item is final or pending.

