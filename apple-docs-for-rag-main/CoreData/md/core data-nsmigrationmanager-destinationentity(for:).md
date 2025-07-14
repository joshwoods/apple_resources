

- Core Data
- NSMigrationManager
-  destinationEntity(for:) 

Instance Method

# destinationEntity(for:)

Returns the entity description for the destination entity of a given entity mapping.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func destinationEntity(for mEntity: NSEntityMapping) -> NSEntityDescription?
```

## Parameters 

`mEntity`  

An entity mapping.

## Return Value

The entity description for the destination entity of `mEntity`.

## Discussion

Entity mappings do not store the actual description objects, but rather the name and version information of the entity.

## See Also

### Getting the Manager’s Configuration

var destinationContext: NSManagedObjectContext

The managed object context the migration manager uses for writing the destination persistent store.

var destinationModel: NSManagedObjectModel

The destination model for the migration manager.

var mappingModel: NSMappingModel

The mapping model for the migration manager.

var sourceContext: NSManagedObjectContext

The managed object context the migration manager uses for reading the source persistent store.

var sourceModel: NSManagedObjectModel

The source model for the migration manager.

func sourceEntity(for: NSEntityMapping) -> NSEntityDescription?

Returns the entity description for the source entity of a given entity mapping.

