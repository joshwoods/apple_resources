

- SwiftData
-  ModelConfiguration 

Structure

# ModelConfiguration

A type that describes the configuration of an app’s schema or specific group of models.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
struct ModelConfiguration
```

## Mentioned in 

Syncing model data across a person’s devices

Preserving your app’s model data across launches

## Topics

### Creating a model configuration

init(isStoredInMemoryOnly: Bool)

Creates a basic model configuration.

init(for: any PersistentModel.Type..., isStoredInMemoryOnly: Bool)

Creates a model configuration for the specified model types.

init(String?, schema: Schema?, isStoredInMemoryOnly: Bool, allowsSave: Bool, groupContainer: ModelConfiguration.GroupContainer, cloudKitDatabase: ModelConfiguration.CloudKitDatabase)

Creates a named model configuration for the specified schema.

init(String?, schema: Schema?, url: URL, allowsSave: Bool, cloudKitDatabase: ModelConfiguration.CloudKitDatabase)

Creates a named model configuration that specifies the on-disk location of the schema’s persistent storage.

### Accessing configuration details

let url: URL

The on-disk location of the schema’s persistent storage.

let name: String

The model configuration’s name.

let allowsSave: Bool

A Boolean value that determines whether the associated persistent storage is writable.

let isStoredInMemoryOnly: Bool

A Boolean value that determines whether the associated persistent storage is ephemeral and exists only in memory.

### Managing schema information

var schema: Schema?

The schema that maps model classes to the associated data in the persistent storage.

var id: URL

The stable identity of the entity associated with this instance.

typealias ID

A type representing the stable identity of the entity associated with an instance.

### Sharing and syncing the model store

let cloudKitContainerIdentifier: String?

The identifier of the configuration’s CloudKit database container.

let cloudKitDatabase: ModelConfiguration.CloudKitDatabase

The option to use when detecting the container of the preferred CloudKit database.

struct CloudKitDatabase

A type that describes the options for detecting a CloudKit database.

let groupAppContainerIdentifier: String?

The identifier of the configuration’s app group container.

let groupContainer: ModelConfiguration.GroupContainer

The option to use when detecting the preferred app group container.

struct GroupContainer

A type that describes the options for detecting an app group container.

### Hashing

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

### Comparing model configurations

static func == (ModelConfiguration, ModelConfiguration) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

CustomDebugStringConvertible Implementations

DataStoreConfiguration Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- DataStoreConfiguration
- Equatable
- Hashable
- Identifiable

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

class Schema

An object that maps model classes to data in the model store, and helps with the migration of that data between releases.

protocol SchemaMigrationPlan

An interface for describing the evolution of a schema and how to migrate between specific versions.

