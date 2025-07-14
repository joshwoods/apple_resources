

- Core Data
-  NSBatchDeleteResult 

Class

# NSBatchDeleteResult

An object that describes the result of a batch delete request.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSBatchDeleteResult
```

## Topics

### Accessing the Result

var result: Any?

The value the request returns after it executes.

var resultType: NSBatchDeleteRequestResultType

The data type of the request’s result value.

enum NSBatchDeleteRequestResultType

The types of result a batch delete request can provide when it executes.

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

### Data Deletion

class NSBatchDeleteRequest

A request that deletes objects in the SQLite persistent store without loading them into memory.

