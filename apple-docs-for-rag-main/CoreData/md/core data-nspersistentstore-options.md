

- Core Data
- NSPersistentStore
-  options 

Instance Property

# options

The options that Core Data uses to create the store.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var options: [AnyHashable : Any]? { get }
```

## Discussion

See NSPersistentStoreCoordinator for a list of key names for options in this dictionary.

## See Also

### Getting Store Configuration

var configurationName: String

The name of the managed object model configuration that creates the persistent store.

var persistentStoreCoordinator: NSPersistentStoreCoordinator?

The persistent store coordinator that loads the persistent store.

var type: String

The type string of the persistent store.

struct StoreType

The types of persistent stores that Core Data supports.

Persistent Store Types

Persist data through the available store types.

