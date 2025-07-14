

- SwiftData
-  HistoryProviding 

Protocol

# HistoryProviding

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+Swift 5.9+

``` source
protocol HistoryProviding
```

## Topics

### Associated Types

associatedtype HistoryType : HistoryTransaction

**Required**

### Instance Methods

func deleteHistory(HistoryDescriptor&lt;Self.HistoryType>) throws

**Required**

func fetchHistory(HistoryDescriptor&lt;Self.HistoryType>) throws -> [Self.HistoryType]

**Required**

### Type Properties

static var historyType: Self.HistoryType.Type

**Required**

## Relationships

### Conforming Types

- DefaultStore

