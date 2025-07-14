

- Apple Pay on the Web
- ApplePayLineItem
-  type 

Instance Property

# type

A value that indicates whether the line item is final or pending.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
ApplePayLineItemType type;
```

## Discussion

See ApplePayLineItemType for valid values.

The default value is `final`.

Note that if a line item’s type is `pending`, the Apple Pay payment sheet doesn’t display the value in amount, and instead displays “pending”.

If a line item’s type is `final`, the payment sheet displays the value in amount.

## Topics

### Line Item Type

ApplePayLineItemType

A type that indicates whether a line item is final or pending.

## See Also

### Setting line item properties

label

A required value that’s a short, localized description of the line item.

amount

A required value that’s the monetary amount of the line item.

