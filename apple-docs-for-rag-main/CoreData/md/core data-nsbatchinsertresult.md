

- Core Data
-  NSBatchInsertResult 

Class

# NSBatchInsertResult

The result that Core Data returns when executing a batch-insertion request.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class NSBatchInsertResult
```

## Topics

### Accessing Results

var result: Any?

The result of a batch-insertion request.

var resultType: NSBatchInsertRequestResultType

The type of result that Core Data returns from this request.

enum NSBatchInsertRequestResultType

Result types for a batch-insertion request.

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

### Data Inserts

class NSBatchInsertRequest

A request to insert a batch of data in a persistent store.

