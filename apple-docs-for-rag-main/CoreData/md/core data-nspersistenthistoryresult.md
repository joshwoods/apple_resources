

- Core Data
-  NSPersistentHistoryResult 

Class

# NSPersistentHistoryResult

The result of a request to fetch persistent history.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class NSPersistentHistoryResult
```

## Mentioned in 

Consuming relevant store changes

## Topics

### Inspecting History Results

var result: Any?

The result of the history request determined by the persistent history result type.

var resultType: NSPersistentHistoryResultType

The type of result that the persistent history change request returns.

enum NSPersistentHistoryResultType

The types of results from a persistent history change request.

## Relationships

### Inherits From

- NSPersistentStoreResult

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Requesting History

class NSPersistentHistoryChangeRequest

A request to fetch or purge persistent history.

