

- Core Data
- NSMigrationManager
-  migrateStore(from:sourceType:options:with:toDestinationURL:destinationType:destinationOptions:) Deprecated

Instance Method

# migrateStore(from:sourceType:options:with:toDestinationURL:destinationType:destinationOptions:)

Migrates the store at a given source URL to the store at a given destination URL, performing all of the mappings specified in a given mapping model.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func migrateStore(
    from sourceURL: URL,
    sourceType sStoreType: String,
    options sOptions: [AnyHashable : Any]? = nil,
    with mappings: NSMappingModel?,
    toDestinationURL dURL: URL,
    destinationType dStoreType: String,
    destinationOptions dOptions: [AnyHashable : Any]? = nil
) throws
```

Deprecated

Use migrateStore(from:type:options:mapping:to:type:options:) instead.

## Parameters 

`sourceURL`  

The location of an existing persistent store. A store must exist at this URL.

`sStoreType`  

The type of store at `sourceURL` (see NSPersistentStoreCoordinator for possible values).

`sOptions`  

A dictionary of options for the source (see NSPersistentStoreCoordinator for possible values).

`mappings`  

The mapping model to use to effect the migration.

`dURL`  

The location of the destination store.

`dStoreType`  

The type of store at `dURL` (see NSPersistentStoreCoordinator for possible values).

`dOptions`  

A dictionary of options for the destination (see NSPersistentStoreCoordinator for possible values).

## Discussion

This method performs compatibility checks on the source and destination models and the mapping model.

### Special Considerations

If a store does not exist at the destination URL (`dURL`), one is created; otherwise, the migration appends to the existing store.

## See Also

### Related Documentation

func cancelMigrationWithError(any Error)

Cancels the migration with a given error.

### Performing a Migration

func migrateStore(from: URL, type: NSPersistentStore.StoreType, options: [AnyHashable : Any]?, mapping: NSMappingModel, to: URL, type: NSPersistentStore.StoreType, options: [AnyHashable : Any]?) throws

Migrates the source store to the destination using the specified mapping model.

