

- Core Data
-  NSCustomMigrationStage 

Class

# NSCustomMigrationStage

An object that enables you to participate in the migration between two versions of the same model.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
class NSCustomMigrationStage
```

## Overview

Use NSCustomMigrationStage when you have two versions of a model that Core Data can’t automatically migrate. Custom migration stages enable you to participate in the migration process by assigning handlers that the stage invokes before and after it runs. The handlers provide an opportunity to prepare the persistent store’s data for the upcoming changes before the stage runs, and perform any cleanup tasks afterward.

For example, to support a migration that changes an optional attribute to be nonoptional, you might assign a handler to the stage’s willMigrateHandler property that sets any `nil` instances of that attribute to a default value, thereby ensuring the migration succeeds. To access the store you’re migrating, use the container property of the migration manager that Core Data provides to every handler.

## Topics

### Creating a custom migration stage

convenience init(migratingFrom: NSManagedObjectModelReference, to: NSManagedObjectModelReference)

Creates a custom migration stage with the specified source and destination model references.

class NSManagedObjectModelReference

An object that describes a specific version of an object model.

### Accessing model references

var currentModel: NSManagedObjectModelReference

The reference that represents the migration’s source model.

var nextModel: NSManagedObjectModelReference

The reference that represents the migration’s destination model.

### Assigning event handlers

var willMigrateHandler: ((NSStagedMigrationManager, NSCustomMigrationStage) throws -> Void)?

The handler to execute before the stage runs.

var didMigrateHandler: ((NSStagedMigrationManager, NSCustomMigrationStage) throws -> Void)?

The handler to execute after the stage runs.

## Relationships

### Inherits From

- NSMigrationStage

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Migration stages

class NSLightweightMigrationStage

An object that describes a series of models suitable for lightweight migration.

class NSMigrationStage

An abstract base class for describing an individual stage of a migration.

