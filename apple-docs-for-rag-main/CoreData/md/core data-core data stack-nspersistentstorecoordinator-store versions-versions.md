

- Core Data
- Core Data stack
- NSPersistentStoreCoordinator
-  Store versions 

API Collection

# Store versions

The metadata keys you use when comparing store versions.

## Topics

### Constants

let NSStoreModelVersionHashesKey: String

Key to represent the version hash information for the model used to create the store.

let NSStoreModelVersionIdentifiersKey: String

Key to represent the version identifiers for the model used to create the store.

let NSPersistentStoreOSCompatibility: String

Key to represent the earliest version of the operation system that the persistent store supports.

## See Also

### Creating a persistent store coordinator

init(managedObjectModel: NSManagedObjectModel)

Creates a persistent store coordinator with the specified managed object model.

Store options

The options keys that configure the behavior and characteristics of a persistent store.

Migration options

The options keys that configure the migration behavior of a persistent store.

