

- Apple Pay on the Web
- ApplePayLineItem
-  label 

Instance Property

# label

A required value that’s a short, localized description of the line item.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
DOMString label;
```

## Discussion

Provide the label in title case—for example, VAT Tax, Gift Wrap and Card, or Discount. The label can’t be empty.

Omit any punctuation and whitespace after the label. The framework formats the label for display.

## See Also

### Setting line item properties

amount

A required value that’s the monetary amount of the line item.

type

A value that indicates whether the line item is final or pending.

