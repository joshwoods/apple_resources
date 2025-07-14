

- FinanceKit
-  FullyQualifiedOrderIdentifier 

Structure

# FullyQualifiedOrderIdentifier

A structure that specifies the characteristics of an order.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
struct FullyQualifiedOrderIdentifier
```

## Topics

### Operators

static func == (FullyQualifiedOrderIdentifier, FullyQualifiedOrderIdentifier) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

init(orderTypeIdentifier: String, orderIdentifier: String)

Initializes the object with values that uniquely identify an order within an order type.

### Instance Properties

var hashValue: Int

The hash value.

var orderIdentifier: String

A string the merchant uses to identify a specific customer order.

var orderTypeIdentifier: String

A string that describes the order type.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

CustomStringConvertible Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Orders

struct HistoryToken

A structure that describes the starting point to use for financial data queries.

func saveOrder(signedArchive: Data) async throws -> FinanceStore.SaveOrderResult

Adds an order to the store or updates an existing order.

