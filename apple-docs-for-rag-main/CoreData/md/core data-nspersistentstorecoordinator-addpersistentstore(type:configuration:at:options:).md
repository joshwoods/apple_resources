

- Core Data
- NSPersistentStoreCoordinator
-  addPersistentStore(type:configuration:at:options:) 

Instance Method

# addPersistentStore(type:configuration:at:options:)

Adds a specific type of persistent store at the provided location.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func addPersistentStore(
    type: NSPersistentStore.StoreType,
    configuration: String? = nil,
    at storeURL: URL,
    options: [AnyHashable : Any]? = nil
) throws -> NSPersistentStore
```

## Parameters 

`type`  

The store type. For possible values, see NSPersistentStore.StoreType.

`configuration`  

The name of the configuration to use. You must define this configuration in the coordinator’s managed object model.

`storeURL`  

The store’s location.

`options`  

A dictionary containing key-value pairs that specify store behavior and characteristics. For more information, see Store options.

## See Also

### Adding or removing a store

func addPersistentStore(ofType: String, configurationName: String?, at: URL?, options: [AnyHashable : Any]?) throws -> NSPersistentStore

Adds a specific type of persistent store at the provided location.

Deprecated

func addPersistentStore(with: NSPersistentStoreDescription, completionHandler: (NSPersistentStoreDescription, (any Error)?) -> Void)

Adds a persistent store using the provided description.

func remove(NSPersistentStore) throws

Removes the specified persistent store from the coordinator.

