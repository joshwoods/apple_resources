

- Apple Pay on the Web
- ApplePayPaymentRequest
-  total 

Instance Property

# total

A line item that represents the total for the payment.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
required ApplePayLineItem total;
```

## Mentioned in 

Apple Pay on the Web Version 4 Release Notes

## Discussion

See ApplePayLineItem.

The amount of the `total` must be greater than or equal to zero and the label must be non-empty to pass validation.

Provide a business name in the label field. Use the same business name people see when they look for the charge on their bank or credit card statement, for example, `“COMPANY, INC."`.

```
"total": {
    "label": "COMPANY, INC.",
    "type": "final",
    "amount": "38.06"
}
```

Note

In versions of Apple Pay JS prior to version 4, the `amount` of the `total` must be greater than zero. Check for version availability using supportsVersion before setting a zero `amount`.

## See Also

### Setting the total and summary line items

lineItems

A set of line items that explain recurring payments and additional charges and discounts.

ApplePayLineItem

A line item in a payment request—for example, total, tax, discount, or grand total.

ApplePayLineItemType

A type that indicates whether a line item is final or pending.

