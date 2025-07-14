

- SwiftData
-  DefaultHistoryUpdate 

Structure

# DefaultHistoryUpdate

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+Swift 5.9+

``` source
struct DefaultHistoryUpdate where Model : PersistentModel
```

## Topics

### Operators

static func == (DefaultHistoryUpdate&lt;Model>, DefaultHistoryUpdate&lt;Model>) -> Bool

### Instance Properties

let changeIdentifier: DefaultHistoryUpdate&lt;Model>.ChangeIdentifier

let changedPersistentIdentifier: PersistentIdentifier

let transactionIdentifier: DefaultHistoryUpdate&lt;Model>.TransactionIdentifier

let updatedAttributes: [any PartialKeyPath&lt;Model> &amp; Sendable]

### Instance Methods

func hash(into: inout Hasher)

### Type Aliases

typealias ChangeIdentifier

typealias PropertyUpdate

typealias TransactionIdentifier

## Relationships

### Conforms To

- HistoryUpdate
- Sendable

