

- Core Data
- NSMigrationManager
-  init(sourceModel:destinationModel:) 

Initializer

# init(sourceModel:destinationModel:)

Initializes a migration manager instance with given source and destination models.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init(
    sourceModel: NSManagedObjectModel,
    destinationModel: NSManagedObjectModel
)
```

## Parameters 

`sourceModel`  

The source managed object model for the migration manager.

`destinationModel`  

The destination managed object model for the migration manager.

## Return Value

A migration manager instance initialized to migrate data in a store that uses `sourceModel` to a store that uses `destinationModel`.

## Discussion

You specify the mapping model in the migration method, migrateStore(from:sourceType:options:with:toDestinationURL:destinationType:destinationOptions:).

### Special Considerations

This is the designated initializer for `NSMigrationManager`.

Although validation of the models is performed during migrateStore(from:sourceType:options:with:toDestinationURL:destinationType:destinationOptions:), as with `NSPersistentStoreCoordinator` once models are added to the migration manager they are immutable and cannot be altered.

## See Also

### Related Documentation

var destinationModel: NSManagedObjectModel

The destination model for the migration manager.

var mappingModel: NSMappingModel

The mapping model for the migration manager.

var sourceModel: NSManagedObjectModel

The source model for the migration manager.

func migrateStore(from: URL, sourceType: String, options: [AnyHashable : Any]?, with: NSMappingModel?, toDestinationURL: URL, destinationType: String, destinationOptions: [AnyHashable : Any]?) throws

Migrates the store at a given source URL to the store at a given destination URL, performing all of the mappings specified in a given mapping model.

Deprecated

Core Data Model Versioning and Data Migration Programming Guide

