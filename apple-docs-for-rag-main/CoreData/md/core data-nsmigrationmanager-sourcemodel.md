

- Core Data
- NSMigrationManager
-  sourceModel 

Instance Property

# sourceModel

The source model for the migration manager.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var sourceModel: NSManagedObjectModel { get }
```

## See Also

### Related Documentation

init(sourceModel: NSManagedObjectModel, destinationModel: NSManagedObjectModel)

Initializes a migration manager instance with given source and destination models.

### Getting the Manager’s Configuration

var destinationContext: NSManagedObjectContext

The managed object context the migration manager uses for writing the destination persistent store.

var destinationModel: NSManagedObjectModel

The destination model for the migration manager.

var mappingModel: NSMappingModel

The mapping model for the migration manager.

var sourceContext: NSManagedObjectContext

The managed object context the migration manager uses for reading the source persistent store.

func destinationEntity(for: NSEntityMapping) -> NSEntityDescription?

Returns the entity description for the destination entity of a given entity mapping.

func sourceEntity(for: NSEntityMapping) -> NSEntityDescription?

Returns the entity description for the source entity of a given entity mapping.

