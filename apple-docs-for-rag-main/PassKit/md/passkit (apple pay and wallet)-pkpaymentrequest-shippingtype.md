

- PassKit (Apple Pay and Wallet)
- PKPaymentRequest
-  shippingType 

Instance Property

# shippingType

The type of shipping the request uses.

iOS 8.3+iPadOS 8.3+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
var shippingType: PKShippingType { get set }
```

## Mentioned in 

Displaying a Read-Only Pickup Address

## Discussion

This property sets the labels for the shipping information displayed by the PKPaymentAuthorizationViewController class. The default value is PKShippingType.shipping. For a complete list of valid shipping types, see PKShippingType.

Note

In iOS 14 and earlier, watchOS 4 and earlier, and Catalyst 14 and earlier, if you’re using a PKShippingType.storePickup shipping type, you need to manage the shipping information displayed by the payment authorization view controller. By default, the system displays the user’s preferred shipping address. You can set the request’s shippingAddress property to the address for your store, or hide the shipping information entirely by setting the requiredShippingAddressFields property to PKAddressFieldNone.

## See Also

### Setting the shipping methods and types

Displaying a Read-Only Pickup Address

Configure a payment request to display a read-only pickup address on the payment sheet.

var shippingMethods: [PKShippingMethod]?

An array of shipping method objects that describe the supported shipping methods.

class PKShippingMethod

An object that defines a shipping method for delivering physical goods.

var shippingContactEditingMode: PKShippingContactEditingMode

A value that indicates whether the shipping mode prevents the user from editing the shipping address.

enum PKShippingType

A complete list of valid shipping types.

enum PKShippingContactEditingMode

Constants that indicate whether the shipping mode prevents the user from editing fields of the shipping address.

