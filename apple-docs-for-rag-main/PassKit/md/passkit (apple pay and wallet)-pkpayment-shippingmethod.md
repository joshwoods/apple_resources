

- PassKit (Apple Pay and Wallet)
- PKPayment
-  shippingMethod 

Instance Property

# shippingMethod

The user-selected shipping method for this transaction.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
var shippingMethod: PKShippingMethod? { get }
```

## Discussion

A value is set for this property only if the corresponding payment request specified available shipping methods in the shippingMethods property of the PKPaymentRequest object. Otherwise, the value is `nil.`

## See Also

### Working with billing and shipping information

var billingContact: PKContact?

The user-selected billing address for this transaction.

var shippingContact: PKContact?

The user-selected shipping address for this transaction.

class PKContact

An object that encapsulates contact information needed for billing and shipping.

class PKShippingMethod

An object that defines a shipping method for delivering physical goods.

