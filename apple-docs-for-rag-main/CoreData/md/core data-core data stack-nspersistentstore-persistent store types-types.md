

- Core Data
- Core Data stack
- NSPersistentStore
-  Persistent Store Types 

API Collection

# Persistent Store Types

Persist data through the available store types.

## Topics

### Constants

let NSSQLiteStoreType: String

The SQLite database store type.

let NSXMLStoreType: String

The XML store type.

let NSBinaryStoreType: String

The binary store type.

let NSInMemoryStoreType: String

The in-memory store type.

## See Also

### Getting Store Configuration

var configurationName: String

The name of the managed object model configuration that creates the persistent store.

var options: [AnyHashable : Any]?

The options that Core Data uses to create the store.

var persistentStoreCoordinator: NSPersistentStoreCoordinator?

The persistent store coordinator that loads the persistent store.

var type: String

The type string of the persistent store.

struct StoreType

The types of persistent stores that Core Data supports.

