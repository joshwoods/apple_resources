

- SwiftData
-  HistoryToken 

Protocol

# HistoryToken

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+Swift 5.9+

``` source
protocol HistoryToken : Comparable, Decodable, Encodable, Hashable, Identifiable, Sendable
```

## Topics

### Associated Types

associatedtype TokenType : Decodable, Encodable, Hashable, Sendable

**Required**

### Instance Properties

var tokenValue: Self.TokenType?

**Required**

## Relationships

### Inherits From

- Comparable
- Decodable
- Encodable
- Equatable
- Hashable
- Identifiable
- Sendable

### Conforming Types

- DefaultHistoryToken

