

- Core Data
-  NSEntityMigrationPolicy 

Class

# NSEntityMigrationPolicy

A policy instance that customizes the migration process for an entity mapping.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class NSEntityMigrationPolicy
```

## Overview

You set the policy for an entity mapping by passing the name of the migration policy class as the argument to entityMigrationPolicyClassName. Typically, you specify the name in the Xcode mapping model editor.

## Topics

### Customizing Stages of the Mapping Life Cycle

func begin(NSEntityMapping, with: NSMigrationManager) throws

Sets up state information before the start of a given entity mapping.

func createDestinationInstances(forSource: NSManagedObject, in: NSEntityMapping, manager: NSMigrationManager) throws

Creates the destination instance(s) for a given source instance.

func endInstanceCreation(forMapping: NSEntityMapping, manager: NSMigrationManager) throws

Indicates the end of the instance creation stage for the specified entity mapping, and the precursor to the next migration stage.

func createRelationships(forDestination: NSManagedObject, in: NSEntityMapping, manager: NSMigrationManager) throws

Constructs the relationships between the newly-created destination instances.

func endRelationshipCreation(forMapping: NSEntityMapping, manager: NSMigrationManager) throws

Indicates the end of the relationship creation stage for the specified entity mapping.

func performCustomValidation(forMapping: NSEntityMapping, manager: NSMigrationManager) throws

Provides the option to perform custom validation on migrated objects during the validation stage of the entity migration policy.

func end(NSEntityMapping, manager: NSMigrationManager) throws

Performs cleanup at the end of the migration, from any phase of the mapping.

### Constants

let NSMigrationManagerKey: String

Key for the migration manager.

let NSMigrationSourceObjectKey: String

Key for the source object.

let NSMigrationDestinationObjectKey: String

Key for the destination object.

let NSMigrationEntityMappingKey: String

Key for the entity mapping object.

let NSMigrationPropertyMappingKey: String

Key for the property mapping object.

let NSMigrationEntityPolicyKey: String

Key for the entity migration policy object.

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

enum NSEntityMappingType

The types for mapping an entity between a source model and a destination model.

class NSPropertyMapping

A mapping instance that specifies in a model how to map from a property in a source entity to a property in a destination entity.

