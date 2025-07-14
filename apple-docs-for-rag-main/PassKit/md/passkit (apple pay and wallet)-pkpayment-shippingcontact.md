

- PassKit (Apple Pay and Wallet)
- PKPayment
-  shippingContact 

Instance Property

# shippingContact

The user-selected shipping address for this transaction.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
var shippingContact: PKContact? { get }
```

## Discussion

Only the fields specified in the requiredShippingAddressFields property of the PKPaymentRequest object are populated. If no required shipping fields were specified, the value of this property is `nil`.

## See Also

### Working with billing and shipping information

var billingContact: PKContact?

The user-selected billing address for this transaction.

var shippingMethod: PKShippingMethod?

The user-selected shipping method for this transaction.

class PKContact

An object that encapsulates contact information needed for billing and shipping.

class PKShippingMethod

An object that defines a shipping method for delivering physical goods.

