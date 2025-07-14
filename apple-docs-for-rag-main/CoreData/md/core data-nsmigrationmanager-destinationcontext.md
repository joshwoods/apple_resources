

- Core Data
- NSMigrationManager
-  destinationContext 

Instance Property

# destinationContext

The managed object context the migration manager uses for writing the destination persistent store.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var destinationContext: NSManagedObjectContext { get }
```

## Discussion

This context is created on demand as part of the initialization of the Core Data stacks used for migration.

## See Also

### Getting the Manager’s Configuration

var destinationModel: NSManagedObjectModel

The destination model for the migration manager.

var mappingModel: NSMappingModel

The mapping model for the migration manager.

var sourceContext: NSManagedObjectContext

The managed object context the migration manager uses for reading the source persistent store.

var sourceModel: NSManagedObjectModel

The source model for the migration manager.

func destinationEntity(for: NSEntityMapping) -> NSEntityDescription?

Returns the entity description for the destination entity of a given entity mapping.

func sourceEntity(for: NSEntityMapping) -> NSEntityDescription?

Returns the entity description for the source entity of a given entity mapping.

