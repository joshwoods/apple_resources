

- Core Data
-  NSBatchUpdateResult 

Class

# NSBatchUpdateResult

The result returned when executing a batch update request.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class NSBatchUpdateResult
```

## Topics

### Accessing Results

var result: Any?

The result of a batch-update request, either the number of updated objects, the identifiers of the updated objects, or a status value.

var resultType: NSBatchUpdateRequestResultType

The type of result that Core Data returns from the request.

enum NSBatchUpdateRequestResultType

Result types for a batch-update request.

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

### Data Updates

class NSBatchUpdateRequest

A request to Core Data to do a batch update of data in a persistent store without loading any data into memory.

