

- SwiftData
-  HistoryUpdate 

Protocol

# HistoryUpdate

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+Swift 5.9+

``` source
protocol HistoryUpdate : Sendable
```

## Topics

### Associated Types

associatedtype ChangeIdentifier : Comparable, Hashable, Sendable

**Required**

associatedtype Model : PersistentModel

**Required**

associatedtype TransactionIdentifier : Comparable, Hashable, Sendable

**Required**

### Instance Properties

var changeIdentifier: Self.ChangeIdentifier

**Required**

var changedPersistentIdentifier: PersistentIdentifier

**Required**

var transactionIdentifier: Self.TransactionIdentifier

**Required**

var updatedAttributes: [any PartialKeyPath&lt;Self.Model> &amp; Sendable]

**Required**

### Type Aliases

typealias PropertyUpdate

## Relationships

### Inherits From

- Sendable

### Conforming Types

- DefaultHistoryUpdate

