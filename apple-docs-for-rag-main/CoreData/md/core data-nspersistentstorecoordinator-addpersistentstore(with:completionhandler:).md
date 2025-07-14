

- Core Data
- NSPersistentStoreCoordinator
-  addPersistentStore(with:completionHandler:) 

Instance Method

# addPersistentStore(with:completionHandler:)

Adds a persistent store using the provided description.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func addPersistentStore(
    with storeDescription: NSPersistentStoreDescription,
    completionHandler block: @escaping (NSPersistentStoreDescription, (any Error)?) -> Void
)
```

## Parameters 

`storeDescription`  

A description object used to create and load a persistent store.

`block`  

The completion handler block that’s invoked after the store is added.

## See Also

### Adding or removing a store

func addPersistentStore(type: NSPersistentStore.StoreType, configuration: String?, at: URL, options: [AnyHashable : Any]?) throws -> NSPersistentStore

Adds a specific type of persistent store at the provided location.

func addPersistentStore(ofType: String, configurationName: String?, at: URL?, options: [AnyHashable : Any]?) throws -> NSPersistentStore

Adds a specific type of persistent store at the provided location.

Deprecated

func remove(NSPersistentStore) throws

Removes the specified persistent store from the coordinator.

