

- Apple Pay on the Web
- ApplePayPaymentRequest
-  lineItems 

Instance Property

# lineItems

A set of line items that explain recurring payments and additional charges and discounts.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
sequence  lineItems;
```

## Discussion

See ApplePayLineItem.

Use lineItems to explain additional charges, discounts, and pending costs. Provide the total separately, in the total property. Line items aren’t required in a ApplePayPaymentRequest, but can’t be empty if they’re present.

The following listing shows line items that include a subtotal, free shipping, and estimated tax.

```
"lineItems": [
    {
        "label": "Bag Subtotal",
        "type": "final",
        "amount": "35.00"
    },
    {
        "label": "Free Shipping",
        "amount": "0.00",
        "type": "final"
    },
    {
        "label": "Estimated Tax",
        "amount": "3.06",
        "type": "final"
    }
]
```

The resulting payment sheet looks like:

## See Also

### Setting the total and summary line items

total

A line item that represents the total for the payment.

ApplePayLineItem

A line item in a payment request—for example, total, tax, discount, or grand total.

ApplePayLineItemType

A type that indicates whether a line item is final or pending.

