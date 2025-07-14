

- Core Data
-  NSMigrationManager 

Class

# NSMigrationManager

A migration manager instance that performs a migration of data from one persistent store to another using a given mapping model.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class NSMigrationManager
```

## Topics

### Creating a Migration Manager

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

var sourceModel: NSManagedObjectModel

The source model for the migration manager.

func destinationEntity(for: NSEntityMapping) -> NSEntityDescription?

Returns the entity description for the destination entity of a given entity mapping.

func sourceEntity(for: NSEntityMapping) -> NSEntityDescription?

Returns the entity description for the source entity of a given entity mapping.

### Customizing the Manager

var userInfo: [AnyHashable : Any]?

The user info for the migration manager.

var usesStoreSpecificMigrationManager: Bool

A Boolean value that indicates whether the migration manager tries to use a store specific migration manager to perform the migration.

### Managing Sources and Destinations

func associate(sourceInstance: NSManagedObject, withDestinationInstance: NSManagedObject, for: NSEntityMapping)

Associates a given source managed object instance with an array of destination instances for a given property mapping.

func destinationInstances(forEntityMappingName: String, sourceInstances: [NSManagedObject]?) -> [NSManagedObject]

Returns the managed object instances created in the destination store for the named entity mapping for the given array of source instances.

func sourceInstances(forEntityMappingName: String, destinationInstances: [NSManagedObject]?) -> [NSManagedObject]

Returns the managed object instances in the source store used to create the given destination instances for the passed in property mapping.

### Performing a Migration

func migrateStore(from: URL, type: NSPersistentStore.StoreType, options: [AnyHashable : Any]?, mapping: NSMappingModel, to: URL, type: NSPersistentStore.StoreType, options: [AnyHashable : Any]?) throws

Migrates the source store to the destination using the specified mapping model.

func migrateStore(from: URL, sourceType: String, options: [AnyHashable : Any]?, with: NSMappingModel?, toDestinationURL: URL, destinationType: String, destinationOptions: [AnyHashable : Any]?) throws

Migrates the store at a given source URL to the store at a given destination URL, performing all of the mappings specified in a given mapping model.

Deprecated

### Monitoring a Migration’s Progress

var migrationProgress: Float

A number between `0` and `1` that indicates the proportion of completeness of the migration.

var currentEntityMapping: NSEntityMapping

The entity mapping currently being processed.

### Aborting a Migration

func cancelMigrationWithError(any Error)

Cancels the migration with a given error.

func reset()

Resets the association tables for the migration.

### Deprecated

Deprecated Symbols

Review unsupported symbols and their replacements.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Entity Mapping

class NSMappingModel

A model instance that specifies how to map a model from a source to a destination managed object model.

class NSEntityMapping

A mapping instance that specifies how to map an entity from a source to a destination managed object model.

class NSEntityMigrationPolicy

A policy instance that customizes the migration process for an entity mapping.

enum NSEntityMappingType

The types for mapping an entity between a source model and a destination model.

class NSPropertyMapping

A mapping instance that specifies in a model how to map from a property in a source entity to a property in a destination entity.

