

- PassKit (Apple Pay and Wallet)
- PKPaymentRequest
-  shippingContact 

Instance Property

# shippingContact

A prepopulated shipping address.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
var shippingContact: PKContact? { get set }
```

## Mentioned in 

Displaying a Read-Only Pickup Address

## Discussion

If you have an up-to-date shipping address on file, you can set this property to that address. This shipping address appears in the payment sheet. When the framework presents the PKPaymentAuthorizationViewController, the user can either keep the address you specified or enter a different address.

Note that a PKContact object that represents a shipping contact contains information for only the postalAddress, emailAddress, and phoneNumber properties. The framework sets all other properties in the object to `nil`.

## See Also

### Providing known contact information

var billingContact: PKContact?

A prepopulated billing address.

class PKContact

An object that encapsulates contact information needed for billing and shipping.

