

- SwiftData
- Schema
-  init(\_:version:) 

Initializer

# init(\_:version:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
init(
    _ entities: Schema.Entity...,
    version: Schema.Version = Version(1, 0, 0)
)
```

## See Also

### Creating a schema

init([any PersistentModel.Type], version: Schema.Version)

convenience init(versionedSchema: any VersionedSchema.Type)

protocol VersionedSchema

An interface for describing a specific version of a schema, including the models it contains.

init()

Schema components

Specify the constituent parts of your schema, including entities, attributes, and relationships.

