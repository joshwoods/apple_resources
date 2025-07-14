

- SwiftData
-  Schema 

Class

# Schema

An object that maps model classes to data in the model store, and helps with the migration of that data between releases.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
final class Schema
```

## Topics

### Creating a schema

init(Schema.Entity..., version: Schema.Version)

init([any PersistentModel.Type], version: Schema.Version)

convenience init(versionedSchema: any VersionedSchema.Type)

protocol VersionedSchema

An interface for describing a specific version of a schema, including the models it contains.

init()

Schema components

Specify the constituent parts of your schema, including entities, attributes, and relationships.

### Accessing entities

let entities: [Schema.Entity]

let entitiesByName: [String : Schema.Entity]

class Entity

An object that provides a blueprint for the associated model class.

### Accessing version details

static let schemaEncodingVersion: Schema.Version

let encodingVersion: Schema.Version

### Saving and loading

func save(to: URL) throws

static func load(from: URL) throws -> Schema

### Encoding and decoding

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Hashing

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Comparing schemas

static func == (Schema, Schema) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Classes

class Index

class Unique

### Structures

struct PropertyMetadata

struct Version

### Instance Properties

var hashValue: Int

The hash value.

let version: Schema.Version

### Instance Methods

func entity&lt;T>(for: T.Type) -> Schema.Entity?

### Type Methods

static func entityName&lt;T>(for: T.Type) -> String

### Default Implementations

CustomDebugStringConvertible Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable

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

protocol SchemaMigrationPlan

An interface for describing the evolution of a schema and how to migrate between specific versions.

