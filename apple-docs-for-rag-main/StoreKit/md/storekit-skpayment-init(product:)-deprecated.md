

- StoreKit
- SKPayment
-  init(product:) Deprecated

Initializer

# init(product:)

Returns a new payment for the specified product.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
convenience init(product: SKProduct)
```

Deprecated

Use Product.purchase(confirmIn:options:)

## Parameters 

`product`  

The product the user wishes to purchase.

## Return Value

A new payment object.

## Discussion

This Object creation uses the `productIdentifier` property obtained from the `product` parameter to create and return a new payment with that identifier. The quantity property defaults to `1`.

To create a SKPayment object with a quantity greater than `1`, create a `SKMutablePayment` object, adjust its `quantity` property and then add it to the payment queue.

```
SKMutablePayment *myPayment = [SKMutablePayment paymentWithProduct: myProduct];
myPayment.quantity = 2;
[[SKPaymentQueue defaultQueue] addPayment:myPayment];
```

## See Also

### Related Documentation

In-App Purchase Programming Guide

