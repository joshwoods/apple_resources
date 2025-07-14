

- Core Data
- NSPersistentStore
-  persistentStoreCoordinator 

Instance Property

# persistentStoreCoordinator

The persistent store coordinator that loads the persistent store.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
weak var persistentStoreCoordinator: NSPersistentStoreCoordinator? { get }
```

## See Also

### Getting Store Configuration

var configurationName: String

The name of the managed object model configuration that creates the persistent store.

var options: [AnyHashable : Any]?

The options that Core Data uses to create the store.

var type: String

The type string of the persistent store.

struct StoreType

The types of persistent stores that Core Data supports.

Persistent Store Types

Persist data through the available store types.

