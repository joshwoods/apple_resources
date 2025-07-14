

- Apple Pay on the Web
-  ApplePayLineItemType 

Enumeration

# ApplePayLineItemType

A type that indicates whether a line item is final or pending.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
enum ApplePayLineItemType
```

## Overview

The constant values are:

`final`  
A line item representing the known, final cost.

`pending`  
A line item representing an estimated or unknown cost.

## Topics

### Enumeration Cases

final

pending

## See Also

### Setting the total and summary line items

total

A line item that represents the total for the payment.

lineItems

A set of line items that explain recurring payments and additional charges and discounts.

ApplePayLineItem

A line item in a payment request—for example, total, tax, discount, or grand total.

