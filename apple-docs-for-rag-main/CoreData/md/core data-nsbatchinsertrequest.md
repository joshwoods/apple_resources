

- Core Data
-  NSBatchInsertRequest 

Class

# NSBatchInsertRequest

A request to insert a batch of data in a persistent store.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class NSBatchInsertRequest
```

## Topics

### Creating a Request

convenience init(entity: NSEntityDescription, dictionaryHandler: (NSMutableDictionary) -> Bool)

Creates a batch-insertion request for a managed entity, and specifies a closure that provides data dictionaries for insertion.

convenience init(entity: NSEntityDescription, managedObjectHandler: (NSManagedObject) -> Bool)

Creates a batch-insertion request for a managed entity, and specifies a closure that inserts data into the entity.

convenience init(entityName: String, dictionaryHandler: (NSMutableDictionary) -> Bool)

Creates a batch-insertion request for a named managed entity, and specifies a closure that provides data dictionaries for insertion.

convenience init(entityName: String, managedObjectHandler: (NSManagedObject) -> Bool)

Creates a batch-insertion request for a named managed entity, and specifies a closure that inserts data into the entity.

init(entity: NSEntityDescription, objects: [[String : Any]])

Creates a batch-insertion request for a managed entity, and provides an array of data dictionaries for insertion.

init(entityName: String, objects: [[String : Any]])

Creates a batch-insertion request for a named managed entity, and provides an array of data dictionaries for insertion.

convenience init()

Creates a Core Data batch-insertion request.

Deprecated

### Configuring a Request

var dictionaryHandler: ((NSMutableDictionary) -> Bool)?

A closure that provides a dictionary for your app to insert data into.

var entity: NSEntityDescription?

The managed entity to insert data into.

var entityName: String

The name of the managed entity to insert data into.

var managedObjectHandler: ((NSManagedObject) -> Bool)?

A closure that provides a managed object for your app to insert data into.

var objectsToInsert: [[String : Any]]?

An array of dictionaries that represents the objects to insert with the keys as attribute names and their assigned values.

var resultType: NSBatchInsertRequestResultType

The type of result that Core Data returns from this request.

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

### Data Inserts

class NSBatchInsertResult

The result that Core Data returns when executing a batch-insertion request.

