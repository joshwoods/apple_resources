

- Core Data
- NSCoreDataCoreSpotlightDelegate
-  init(forStoreWith:model:) Deprecated

Initializer

# init(forStoreWith:model:)

Creates a Core Spotlight delegate with the specified store description and managed object model.

iOS 11.0–15.0DeprecatediPadOS 11.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.13–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
convenience init(
    forStoreWith description: NSPersistentStoreDescription,
    model: NSManagedObjectModel
)
```

Deprecated

Use init(forStoreWith:coordinator:) instead.

## Parameters 

`description`  

An object that describes the persistent store that contains the entities to index.

`model`  

The managed object model that contains the definitions of the entities to index.

## See Also

### Creating a Core Spotlight Delegate

init(forStoreWith: NSPersistentStoreDescription, coordinator: NSPersistentStoreCoordinator)

Creates a Core Spotlight delegate with the specified store description and coordinator.

