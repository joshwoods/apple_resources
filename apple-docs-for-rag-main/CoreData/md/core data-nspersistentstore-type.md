

- Core Data
- NSPersistentStore
-  type 

Instance Property

# type

The type string of the persistent store.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var type: String { get }
```

## Discussion

This string is used when specifying the type of store to add to a persistent store coordinator.

### Special Considerations

Subclasses must override this method to provide a unique type.

## See Also

### Getting Store Configuration

var configurationName: String

The name of the managed object model configuration that creates the persistent store.

var options: [AnyHashable : Any]?

The options that Core Data uses to create the store.

var persistentStoreCoordinator: NSPersistentStoreCoordinator?

The persistent store coordinator that loads the persistent store.

struct StoreType

The types of persistent stores that Core Data supports.

Persistent Store Types

Persist data through the available store types.

