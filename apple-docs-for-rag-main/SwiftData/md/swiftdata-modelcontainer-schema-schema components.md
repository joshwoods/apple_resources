

- SwiftData
- ModelContainer
- Schema
-  Schema components 

API Collection

# Schema components

Specify the constituent parts of your schema, including entities, attributes, and relationships.

## Topics

### Entities

class Entity

An object that provides a blueprint for the associated model class.

### Attributes

class Attribute

An object that describes the configuration and behavior of a specific property of a model class.

class CompositeAttribute

An object that describes an attribute that derives its value by composing other attributes.

### Relationships

class Relationship

An object that describes the configuration and behavior of a relationship between two model classes.

### Internal

Internal symbols

Restricted-use symbols that the framework requires for macro expansion and other internal tasks.

## See Also

### Creating a schema

init(Schema.Entity..., version: Schema.Version)

init([any PersistentModel.Type], version: Schema.Version)

convenience init(versionedSchema: any VersionedSchema.Type)

protocol VersionedSchema

An interface for describing a specific version of a schema, including the models it contains.

init()

