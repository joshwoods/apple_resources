

- Core Data
-  NSEntityMappingType 

Enumeration

# NSEntityMappingType

The types for mapping an entity between a source model and a destination model.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum NSEntityMappingType
```

## Topics

### Enumeration Cases

case addEntityMappingType

Specifies that this is a new entity in the destination model.

case copyEntityMappingType

Specifies that source instances are migrated as-is.

case customEntityMappingType

Specifies a custom mapping.

case removeEntityMappingType

Specifies that this entity is not present in the destination model.

case transformEntityMappingType

Specifies that entity exists in source and destination and is mapped.

case undefinedEntityMappingType

Specifies that the developer handles destination instance creation.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Entity Mapping

class NSMigrationManager

A migration manager instance that performs a migration of data from one persistent store to another using a given mapping model.

class NSMappingModel

A model instance that specifies how to map a model from a source to a destination managed object model.

class NSEntityMapping

A mapping instance that specifies how to map an entity from a source to a destination managed object model.

class NSEntityMigrationPolicy

A policy instance that customizes the migration process for an entity mapping.

class NSPropertyMapping

A mapping instance that specifies in a model how to map from a property in a source entity to a property in a destination entity.

