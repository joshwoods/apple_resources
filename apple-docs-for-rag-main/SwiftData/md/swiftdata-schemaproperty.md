

- SwiftData
-  SchemaProperty 

Protocol

# SchemaProperty

An interface for describing a property.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
protocol SchemaProperty : Decodable, Encodable, Hashable
```

## Topics

### Instance Properties

var isAttribute: Bool

**Required** Default implementation provided.

var isOptional: Bool

**Required** Default implementation provided.

var isRelationship: Bool

**Required** Default implementation provided.

var isTransient: Bool

**Required** Default implementation provided.

var isUnique: Bool

**Required**

var name: String

**Required**

var originalName: String

**Required**

var valueType: any Any.Type

**Required**

## Relationships

### Inherits From

- Decodable
- Encodable
- Equatable
- Hashable

### Conforming Types

- Schema.Attribute
- Schema.CompositeAttribute
- Schema.Index
- Schema.Relationship
- Schema.Unique

## See Also

### Properties

protocol RelationshipCollection

An interface for describing a collection of related models.

