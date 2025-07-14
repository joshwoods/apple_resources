

- Core Data
-  NSPersistentHistoryResultType 

Enumeration

# NSPersistentHistoryResultType

The types of results from a persistent history change request.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
enum NSPersistentHistoryResultType
```

## Topics

### Result Types

case statusOnly

The status of the persistent history change request.

case count

The number of persistent history changes since the requested date, token, or transaction.

case objectIDs

The identifiers of managed objects changed since the requested date, token, or transaction.

case transactionsAndChanges

The persistent history transactions and changes since the requested date, token, or transaction.

case transactionsOnly

The persistent history transactions since the requested date, token, or transaction.

case changesOnly

The persistent history changes since the requested date, token, or transaction.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting History Results

var result: Any?

The result of the history request determined by the persistent history result type.

var resultType: NSPersistentHistoryResultType

The type of result that the persistent history change request returns.

