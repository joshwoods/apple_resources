

- SwiftData
-  HistoryTransaction 

Protocol

# HistoryTransaction

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+Swift 5.9+

``` source
protocol HistoryTransaction : Hashable, Identifiable, Sendable
```

## Topics

### Associated Types

associatedtype TokenType : Comparable, Hashable, Identifiable, Sendable

**Required**

associatedtype TransactionIdentifier : Comparable, Hashable, Sendable

**Required**

### Instance Properties

var author: String?

**Required**

var changes: [HistoryChange]

**Required**

var storeIdentifier: String

**Required**

var timestamp: Date

**Required**

var token: Self.TokenType

**Required**

var transactionIdentifier: Self.TransactionIdentifier

**Required**

## Relationships

### Inherits From

- Equatable
- Hashable
- Identifiable
- Sendable

### Conforming Types

- DefaultHistoryTransaction

