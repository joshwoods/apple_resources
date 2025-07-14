

- Core Data
- Core Data stack
- NSPersistentStoreCoordinator
-  Migration options 

API Collection

# Migration options

The options keys that configure the migration behavior of a persistent store.

## Topics

### Constants

let NSIgnorePersistentStoreVersioningOption: String

Key to ignore the built-in versioning provided by Core Data.

let NSMigratePersistentStoresAutomaticallyOption: String

Key to automatically attempt to migrate versioned stores.

let NSInferMappingModelAutomaticallyOption: String

Key to attempt to create the mapping model automatically.

## See Also

### Creating a persistent store coordinator

init(managedObjectModel: NSManagedObjectModel)

Creates a persistent store coordinator with the specified managed object model.

Store options

The options keys that configure the behavior and characteristics of a persistent store.

Store versions

The metadata keys you use when comparing store versions.

