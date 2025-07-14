

- PassKit (Apple Pay and Wallet)
-  PKShippingMethod 

Class

# PKShippingMethod

An object that defines a shipping method for delivering physical goods.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
class PKShippingMethod
```

## Topics

### Working with shipping methods

var detail: String?

A user-readable description of the shipping method.

var dateComponentsRange: PKDateComponentsRange?

An expected range of delivery or shipping dates for a package, or the time range when an item is available for pickup.

var identifier: String?

A unique identifier for the shipping method, used by the app.

class PKDateComponentsRange

An object that specifies the start and end dates for a range of time.

## Relationships

### Inherits From

- PKPaymentSummaryItem

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Working with billing and shipping information

var billingContact: PKContact?

The user-selected billing address for this transaction.

var shippingContact: PKContact?

The user-selected shipping address for this transaction.

var shippingMethod: PKShippingMethod?

The user-selected shipping method for this transaction.

class PKContact

An object that encapsulates contact information needed for billing and shipping.

