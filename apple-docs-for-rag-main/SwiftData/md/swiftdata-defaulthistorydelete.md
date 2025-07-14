

- SwiftData
-  DefaultHistoryDelete 

Structure

# DefaultHistoryDelete

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+Swift 5.9+

``` source
struct DefaultHistoryDelete where Model : PersistentModel
```

## Topics

### Operators

static func == (DefaultHistoryDelete&lt;Model>, DefaultHistoryDelete&lt;Model>) -> Bool

### Instance Properties

let changeIdentifier: DefaultHistoryDelete&lt;Model>.ChangeIdentifier

let changedPersistentIdentifier: PersistentIdentifier

let tombstone: HistoryTombstone&lt;Model>

let transactionIdentifier: DefaultHistoryDelete&lt;Model>.TransactionIdentifier

### Instance Methods

func hash(into: inout Hasher)

### Type Aliases

typealias ChangeIdentifier

typealias TransactionIdentifier

## Relationships

### Conforms To

- HistoryDelete
- Sendable

