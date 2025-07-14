

- Core Data
- NSCoreDataCoreSpotlightDelegate
-  init(forStoreWith:coordinator:) 

Initializer

# init(forStoreWith:coordinator:)

Creates a Core Spotlight delegate with the specified store description and coordinator.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
init(
    forStoreWith description: NSPersistentStoreDescription,
    coordinator psc: NSPersistentStoreCoordinator
)
```

## Parameters 

`description`  

An object that describes the persistent store that contains the entities to index.

`psc`  

The persistent store coordinator, which you initialize with the managed object model that contains the definitions of the entities to index.

## Discussion

After you initialize a Core Spotlight delegate, call the startSpotlightIndexing() to begin indexing your store’s contents.

Note

If you initialize your Core Spotlight delegate using this method, you don’t need to set the NSCoreDataCoreSpotlightExporter option on the specified store description.

## See Also

### Creating a Core Spotlight Delegate

convenience init(forStoreWith: NSPersistentStoreDescription, model: NSManagedObjectModel)

Creates a Core Spotlight delegate with the specified store description and managed object model.

Deprecated

