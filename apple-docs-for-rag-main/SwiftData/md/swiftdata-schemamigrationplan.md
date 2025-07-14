

- SwiftData
-  SchemaMigrationPlan 

Protocol

# SchemaMigrationPlan

An interface for describing the evolution of a schema and how to migrate between specific versions.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
protocol SchemaMigrationPlan
```

## Topics

### Managing versioned schemas

static var schemas: [any VersionedSchema.Type]

**Required**

protocol VersionedSchema

An interface for describing a specific version of a schema, including the models it contains.

### Managing migration stages

static var stages: [MigrationStage]

**Required**

enum MigrationStage

Describes a migration between two versions of the same schema.

## See Also

### Creating a model container

init(for: Schema, migrationPlan: (any SchemaMigrationPlan.Type)?, configurations: [ModelConfiguration]) throws

Creates a model container using the specified schema, migration plan, and configurations.

convenience init(for: any PersistentModel.Type..., migrationPlan: (any SchemaMigrationPlan.Type)?, configurations: ModelConfiguration...) throws

Creates a model container using the specified model types, migration plan, and zero or more configurations.

convenience init(for: Schema, migrationPlan: (any SchemaMigrationPlan.Type)?, configurations: ModelConfiguration...) throws

Creates a model container using the specified schema, migration plan, and zero or more configurations.

protocol PersistentModel

An interface that enables SwiftData to manage a Swift class as a stored model.

struct ModelConfiguration

A type that describes the configuration of an app’s schema or specific group of models.

class Schema

An object that maps model classes to data in the model store, and helps with the migration of that data between releases.

