

- SwiftData
-  DefaultHistoryTransaction 

Structure

# DefaultHistoryTransaction

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+Swift 5.9+

``` source
struct DefaultHistoryTransaction
```

## Topics

### Operators

static func == (DefaultHistoryTransaction, DefaultHistoryTransaction) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

let author: String?

let bundleIdentifier: String

let changes: [HistoryChange]

var hashValue: Int

The hash value.

var id: Int64

The stable identity of the entity associated with this instance.

let processIdentifier: String

let storeIdentifier: String

let timestamp: Date

let token: DefaultHistoryTransaction.TokenType

let transactionIdentifier: DefaultHistoryTransaction.TransactionIdentifier

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

typealias TokenType

typealias TransactionIdentifier

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- HistoryTransaction
- Identifiable
- Sendable

