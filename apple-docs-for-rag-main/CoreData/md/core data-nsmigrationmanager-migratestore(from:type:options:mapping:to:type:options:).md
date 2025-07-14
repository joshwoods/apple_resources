

- Core Data
- NSMigrationManager
-  migrateStore(from:type:options:mapping:to:type:options:) 

Instance Method

# migrateStore(from:type:options:mapping:to:type:options:)

Migrates the source store to the destination using the specified mapping model.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func migrateStore(
    from sourceURL: URL,
    type sourceType: NSPersistentStore.StoreType,
    options sourceOptions: [AnyHashable : Any]? = nil,
    mapping: NSMappingModel,
    to destinationURL: URL,
    type destinationType: NSPersistentStore.StoreType,
    options destinationOptions: [AnyHashable : Any]? = nil
) throws
```

## Parameters 

`sourceURL`  

The location of the store to migrate.

`sourceType`  

The persistent store type of the store you’re migrating from. For possible values, see NSPersistentStore.StoreType.

`sourceOptions`  

A dictionary of options to apply to the source store. For possible values, see NSPersistentStoreCoordinator.

`mapping`  

The mapping model that converts the entities in the source store to those in the destination store.

`destinationURL`  

The location of the destination store.

`destinationType`  

The persistent store type of the store you’re migrating to. For possible values, see NSPersistentStore.StoreType.

`destinationOptions`  

A dictionary of options to apply to the destination store. For possible values, see NSPersistentStoreCoordinator.

## Discussion

A store must exist at `sourceURL`; otherwise, the migration fails. Before the migration occurs, the method ensures compatibility between the source model, the destination model, and the mapping model. If a store doesn’t exist at `destinationURL`, Core Data creates one as part of the migration; otherwise, the migration updates the existing store.

## See Also

### Performing a Migration

func migrateStore(from: URL, sourceType: String, options: [AnyHashable : Any]?, with: NSMappingModel?, toDestinationURL: URL, destinationType: String, destinationOptions: [AnyHashable : Any]?) throws

Migrates the store at a given source URL to the store at a given destination URL, performing all of the mappings specified in a given mapping model.

Deprecated

