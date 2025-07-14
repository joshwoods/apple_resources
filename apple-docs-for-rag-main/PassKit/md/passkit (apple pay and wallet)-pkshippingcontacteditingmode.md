

- PassKit (Apple Pay and Wallet)
-  PKShippingContactEditingMode 

Enumeration

# PKShippingContactEditingMode

Constants that indicate whether the shipping mode prevents the user from editing fields of the shipping address.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+watchOS 8.0+

``` source
enum PKShippingContactEditingMode
```

## Topics

### Reading the editing mode

case available

The value that indicates Apple Pay Later is available.

case storePickup

The shipping contact on the payment sheet represents a pickup address and isn’t editable by the user.

### Initializers

init?(rawValue: UInt)

### Type Properties

static var enabled: PKShippingContactEditingMode

All fields of the shipping contact on the payment sheet are editable by the user.

Deprecated

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

enum PKShippingType

A complete list of valid shipping types.

