

- Core Data
-  NSEntityMapping 

Class

# NSEntityMapping

A mapping instance that specifies how to map an entity from a source to a destination managed object model.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class NSEntityMapping
```

## Topics

### Managing Source Information

var sourceEntityName: String?

The source entity name for the entity mapping.

var sourceEntityVersionHash: Data?

The version hash of the source entity for the entity mapping.

var sourceExpression: NSExpression?

The source expression for the entity mapping.

### Managing Destination Information

var destinationEntityName: String?

The destination entity name for the entity mapping.

var destinationEntityVersionHash: Data?

The version hash for the destination entity for the entity mapping.

### Managing Mapping Information

var name: String!

The name of the entity mapping.

var mappingType: NSEntityMappingType

The mapping type for the entity mapping.

var entityMigrationPolicyClassName: String?

The class name of the migration policy for the entity mapping.

var attributeMappings: [NSPropertyMapping]?

The array of attribute mappings for the entity mapping.

var relationshipMappings: [NSPropertyMapping]?

The array of relationship mappings for the entity mapping.

var userInfo: [AnyHashable : Any]?

The user info dictionary for the entity mapping.

### Constants

case undefinedEntityMappingType

Specifies that the developer handles destination instance creation.

case customEntityMappingType

Specifies a custom mapping.

case addEntityMappingType

Specifies that this is a new entity in the destination model.

case removeEntityMappingType

Specifies that this entity is not present in the destination model.

case copyEntityMappingType

Specifies that source instances are migrated as-is.

case transformEntityMappingType

Specifies that entity exists in source and destination and is mapped.

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

class NSMappingModel

A model instance that specifies how to map a model from a source to a destination managed object model.

class NSEntityMigrationPolicy

A policy instance that customizes the migration process for an entity mapping.

enum NSEntityMappingType

The types for mapping an entity between a source model and a destination model.

class NSPropertyMapping

A mapping instance that specifies in a model how to map from a property in a source entity to a property in a destination entity.

