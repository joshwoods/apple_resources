

- Core Data
- NSPersistentStore
-  NSPersistentStore.StoreType 

Structure

# NSPersistentStore.StoreType

The types of persistent stores that Core Data supports.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
struct StoreType
```

## Topics

### Store Types

static let binary: NSPersistentStore.StoreType

A store that reads from and writes to a persistent binary file.

static let inMemory: NSPersistentStore.StoreType

An ephemeral store that reads from and writes to memory only.

static let sqlite: NSPersistentStore.StoreType

A store that reads from and writes to a persistent SQLite database.

static let xml: NSPersistentStore.StoreType

A store that reads from and writes to a persistent XML file.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable

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

Persistent Store Types

Persist data through the available store types.

