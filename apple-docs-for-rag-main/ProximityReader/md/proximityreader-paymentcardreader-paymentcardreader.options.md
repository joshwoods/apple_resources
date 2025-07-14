

- ProximityReader
- PaymentCardReader
-  PaymentCardReader.Options 

Structure

# PaymentCardReader.Options

Additional information you use to configure a payment card reader.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.0+

``` source
struct Options
```

## Topics

### Creating an options structure

init(vasMerchants: [VASRequest.Merchant])

Creates a new options structure with the specified list of merchants.

Deprecated

### Getting the list of merchants

var vasMerchants: [VASRequest.Merchant]

A global list of merchants to use when reading loyalty cards.

Deprecated

### Setting read behaviors

var includeErrorInReadResult: Bool

A Boolean value that indicates whether the framework returns a result instead of throwing an error when some data is retrievable.

var returnReadResultImmediately: Bool

A Boolean value that indicates whether the framework returns a result as soon as possible before closing the system UI.

### Initializers

init()

Creates a new options structure with default values

## Relationships

### Conforms To

- Sendable

## See Also

### Creating a payment reader

init(options: PaymentCardReader.Options)

Creates a payment card reader with the specified options.

