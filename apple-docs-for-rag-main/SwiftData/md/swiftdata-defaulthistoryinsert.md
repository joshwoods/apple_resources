

- SwiftData
-  DefaultHistoryInsert 

Structure

# DefaultHistoryInsert

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+Swift 5.9+

``` source
struct DefaultHistoryInsert where Model : PersistentModel
```

## Topics

### Operators

static func == (DefaultHistoryInsert&lt;Model>, DefaultHistoryInsert&lt;Model>) -> Bool

### Instance Properties

let changeIdentifier: DefaultHistoryInsert&lt;Model>.ChangeIdentifier

let changedPersistentIdentifier: PersistentIdentifier

let transactionIdentifier: DefaultHistoryInsert&lt;Model>.TransactionIdentifier

### Instance Methods

func hash(into: inout Hasher)

### Type Aliases

typealias ChangeIdentifier

typealias TransactionIdentifier

## Relationships

### Conforms To

- HistoryInsert
- Sendable

