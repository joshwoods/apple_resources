

- Core Data
- NSMigrationManager
-  mappingModel 

Instance Property

# mappingModel

The mapping model for the migration manager.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var mappingModel: NSMappingModel { get }
```

## See Also

### Related Documentation

func migrateStore(from: URL, sourceType: String, options: [AnyHashable : Any]?, with: NSMappingModel?, toDestinationURL: URL, destinationType: String, destinationOptions: [AnyHashable : Any]?) throws

Migrates the store at a given source URL to the store at a given destination URL, performing all of the mappings specified in a given mapping model.

Deprecated

### Getting the Manager’s Configuration

var destinationContext: NSManagedObjectContext

The managed object context the migration manager uses for writing the destination persistent store.

var destinationModel: NSManagedObjectModel

The destination model for the migration manager.

var sourceContext: NSManagedObjectContext

The managed object context the migration manager uses for reading the source persistent store.

var sourceModel: NSManagedObjectModel

The source model for the migration manager.

func destinationEntity(for: NSEntityMapping) -> NSEntityDescription?

Returns the entity description for the destination entity of a given entity mapping.

func sourceEntity(for: NSEntityMapping) -> NSEntityDescription?

Returns the entity description for the source entity of a given entity mapping.

