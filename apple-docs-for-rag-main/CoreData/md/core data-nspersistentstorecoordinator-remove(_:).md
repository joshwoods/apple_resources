

- Core Data
- NSPersistentStoreCoordinator
-  remove(\_:) 

Instance Method

# remove(\_:)

Removes the specified persistent store from the coordinator.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func remove(_ store: NSPersistentStore) throws
```

## Parameters 

`store`  

A persistent store.

## See Also

### Related Documentation

func migratePersistentStore(NSPersistentStore, to: URL, options: [AnyHashable : Any]?, withType: String) throws -> NSPersistentStore

Changes the location and, if necessary, the store type of the specified persistent store.

Deprecated

func addPersistentStore(ofType: String, configurationName: String?, at: URL?, options: [AnyHashable : Any]?) throws -> NSPersistentStore

Adds a specific type of persistent store at the provided location.

Deprecated

### Adding or removing a store

func addPersistentStore(type: NSPersistentStore.StoreType, configuration: String?, at: URL, options: [AnyHashable : Any]?) throws -> NSPersistentStore

Adds a specific type of persistent store at the provided location.

func addPersistentStore(ofType: String, configurationName: String?, at: URL?, options: [AnyHashable : Any]?) throws -> NSPersistentStore

Adds a specific type of persistent store at the provided location.

Deprecated

func addPersistentStore(with: NSPersistentStoreDescription, completionHandler: (NSPersistentStoreDescription, (any Error)?) -> Void)

Adds a persistent store using the provided description.

