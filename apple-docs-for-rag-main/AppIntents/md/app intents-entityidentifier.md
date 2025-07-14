

- App Intents
-  EntityIdentifier 

Structure

# EntityIdentifier

A type that uniquely identifies a specific instance of an app entity.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct EntityIdentifier
```

## Overview

The value used should be unique across all entities of the given type. Entities which are relevant across executions of the application should have stable identifiers that persist across executions.

Entities, by default, conform to the `Identifiable` protocol. Use a type for the `id` that conforms to EntityIdentifierConvertible. Default implementations for `String`, `UUID` and `Int` are provided.

For example:

```
struct Song: AppEntity {
    let id = UUID()
}
```

## Topics

### Creating an entity identifier

init&lt;Entity>(for: Entity)

Creates an identifier for the specified entity

init&lt;Entity>(for: Entity.Type, identifier: Entity.ID)

Creates an `EntityIdentifier` representing an instance of the specified entity type backed by the specified identifier value.

### Getting the identifier details

let identifier: String

Value uniquely identifying the entity instance within its type

let entityType: any AppEntity.Type

The type of `AppEntity` represented by this identifier

static let valueMaximumLength: Int

Maximum allowed length for the `identifier` value. This is a constraint imposed by the system and thus forces us to truncate the identifier if it exceeds the maximum length.

### Describing the identifier

var description: String

A textual representation of this instance.

### Providing a hash value

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Operators

static func == (EntityIdentifier, EntityIdentifier) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init?(activityIdentifier: String)

### Instance Properties

var hashValue: Int

The hash value.

### Type Aliases

typealias Specification

typealias UnwrappedType

typealias ValueType

### Type Properties

static var defaultResolverSpecification: EmptyResolverSpecification&lt;EntityIdentifier>

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Entity identity

protocol PersistentlyIdentifiable

Defines a string that uniquely identifies a type. This is useful for maintaining the identity of a type, even when its type name is changed.

protocol EntityIdentifierConvertible

An interface for converting between an entity’s identifier and its string representation.

