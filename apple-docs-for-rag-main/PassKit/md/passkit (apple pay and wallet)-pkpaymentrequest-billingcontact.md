

- PassKit (Apple Pay and Wallet)
- PKPaymentRequest
-  billingContact 

Instance Property

# billingContact

A prepopulated billing address.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
var billingContact: PKContact? { get set }
```

## Discussion

If you have an up-to-date billing address on file, you can set it here. This billing address appears in the payment sheet. The user can either use the address you specify or select a different address.

Note that a PKContact object that represents a billing contact contains information for only the postalAddress property. All other properties in the object are set to `nil`.

## See Also

### Providing known contact information

var shippingContact: PKContact?

A prepopulated shipping address.

class PKContact

An object that encapsulates contact information needed for billing and shipping.

