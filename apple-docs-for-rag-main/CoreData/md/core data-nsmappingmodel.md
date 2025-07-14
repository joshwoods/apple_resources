

- Core Data
-  NSMappingModel 

Class

# NSMappingModel

A model instance that specifies how to map a model from a source to a destination managed object model.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class NSMappingModel
```

## Topics

### Creating a Mapping

init?(from: [Bundle]?, forSourceModel: NSManagedObjectModel?, destinationModel: NSManagedObjectModel?)

Returns the mapping model that will translate data from the source to the destination model.

class func inferredMappingModel(forSourceModel: NSManagedObjectModel, destinationModel: NSManagedObjectModel) throws -> NSMappingModel

Returns a newly created mapping model that will migrate data from the source to the destination model.

init?(contentsOf: URL?)

Returns a mapping model initialized from a given URL.

### Managing Entity Mappings

var entityMappings: [NSEntityMapping]!

The entity mappings for the mapping model.

var entityMappingsByName: [String : NSEntityMapping]

The entity mappings for the mapping model, keyed by name.

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

class NSMigrationManager

A migration manager instance that performs a migration of data from one persistent store to another using a given mapping model.

class NSEntityMapping

A mapping instance that specifies how to map an entity from a source to a destination managed object model.

class NSEntityMigrationPolicy

A policy instance that customizes the migration process for an entity mapping.

enum NSEntityMappingType

The types for mapping an entity between a source model and a destination model.

class NSPropertyMapping

A mapping instance that specifies in a model how to map from a property in a source entity to a property in a destination entity.

