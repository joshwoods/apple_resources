

- Core Data
-  NSPropertyMapping 

Class

# NSPropertyMapping

A mapping instance that specifies in a model how to map from a property in a source entity to a property in a destination entity.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class NSPropertyMapping
```

## Topics

### Managing Mapping Attributes

var name: String?

The name of the property in the destination entity for the property mapping.

var valueExpression: NSExpression?

The value expression for the property mapping.

var userInfo: [AnyHashable : Any]?

The user info for the property mapping.

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

class NSEntityMapping

A mapping instance that specifies how to map an entity from a source to a destination managed object model.

class NSEntityMigrationPolicy

A policy instance that customizes the migration process for an entity mapping.

enum NSEntityMappingType

The types for mapping an entity between a source model and a destination model.

