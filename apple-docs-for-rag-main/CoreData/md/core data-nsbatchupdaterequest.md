

- Core Data
-  NSBatchUpdateRequest 

Class

# NSBatchUpdateRequest

A request to Core Data to do a batch update of data in a persistent store without loading any data into memory.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class NSBatchUpdateRequest
```

## Topics

### Creating a Request

init(entity: NSEntityDescription)

Creates a batch-update request for a managed entity.

init(entityName: String)

Creates a batch-update request for a named managed entity.

### Configuring a Request

var entity: NSEntityDescription

The managed entity to update data for.

var entityName: String

The name of the managed entity to update data for.

var includesSubentities: Bool

A Boolean value that indicates whether to update subentities.

var predicate: NSPredicate?

A predicate that identifies the objects to update.

var propertiesToUpdate: [AnyHashable : Any]?

A dictionary of property description pairs that describe the updates.

var resultType: NSBatchUpdateRequestResultType

The type of result that Core Data returns from the request.

## Relationships

### Inherits From

- NSPersistentStoreRequest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Data Updates

class NSBatchUpdateResult

The result returned when executing a batch update request.

