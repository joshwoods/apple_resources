

- SwiftData
-  VersionedSchema 

Protocol

# VersionedSchema

An interface for describing a specific version of a schema, including the models it contains.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
protocol VersionedSchema
```

## Topics

### Describing the version

static var versionIdentifier: Schema.Version

The textual description of the migration’s version or purpose.

**Required**

### Specifying the included models

static var models: [any PersistentModel.Type]

The models to include in this version of the schema.

**Required**

## See Also

### Creating a schema

init(Schema.Entity..., version: Schema.Version)

init([any PersistentModel.Type], version: Schema.Version)

convenience init(versionedSchema: any VersionedSchema.Type)

init()

Schema components

Specify the constituent parts of your schema, including entities, attributes, and relationships.

