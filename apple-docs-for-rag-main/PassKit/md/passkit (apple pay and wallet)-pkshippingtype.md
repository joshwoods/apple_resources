

- PassKit (Apple Pay and Wallet)
-  PKShippingType 

Enumeration

# PKShippingType

A complete list of valid shipping types.

iOS 8.3+iPadOS 8.3+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
enum PKShippingType
```

## Topics

### Constants

case shipping

Shipping the purchase to the provided address using a third-party shipping company. This is the default shipping type.

case delivery

Delivering the purchase by the seller (for example, pizza, flower, or furniture delivery).

case storePickup

Store pickup of the purchase from the seller’s store.

case servicePickup

Picking up an item from the provided address by the service (for example, transportation or shipping services that provide home pickup).

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Setting the shipping methods and types

Displaying a Read-Only Pickup Address

Configure a payment request to display a read-only pickup address on the payment sheet.

var shippingMethods: [PKShippingMethod]?

An array of shipping method objects that describe the supported shipping methods.

class PKShippingMethod

An object that defines a shipping method for delivering physical goods.

var shippingType: PKShippingType

The type of shipping the request uses.

var shippingContactEditingMode: PKShippingContactEditingMode

A value that indicates whether the shipping mode prevents the user from editing the shipping address.

enum PKShippingContactEditingMode

Constants that indicate whether the shipping mode prevents the user from editing fields of the shipping address.

