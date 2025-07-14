

- App Intents
-  EntityIdentifierConvertible 

Protocol

# EntityIdentifierConvertible

An interface for converting between an entity’s identifier and its string representation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol EntityIdentifierConvertible
```

## Mentioned in 

Integrating custom data types into your intents

## Overview

Every entity provides a stable, unique identifier that the framework uses as a concrete reference to the entity while mediating between your app and other parts of the system. To enforce this requirement, the AppEntity protocol inherits the Identifiable protocol.

Wherever possible, use String, Int, or UUID for an identifier’s type. If you must use a different data type, use this protocol to extend that type and implement the required support. For example, an app that integrates with the MusicKit framework might use MusicItemID as the type for an entity’s identifier.

```
extension MusicItemID: EntityIdentifierConvertible {
    public var entityIdentifierString: String {
        rawValue
    }

    public init?(entityIdentifierString: String) {
        self = MusicItemID(entityIdentifierString)
    }
}
```

Important

Keep your entityIdentifierString to 4096 characters or fewer. Otherwise, the framework truncates the value, and you might not be able to convert the truncated value back to its originating type.

## Topics

### Getting the identifier string

var entityIdentifierString: String

The `AppEntity`’s identifier value as a `String`.

**Required**

### Type Methods

static func entityIdentifier(for: String) -> Self?

Identifiers should be able to initialize via a `String` format.

**Required**

## Relationships

### Conforming Types

- FileEntityIdentifier

## See Also

### Entity identity

protocol PersistentlyIdentifiable

Defines a string that uniquely identifies a type. This is useful for maintaining the identity of a type, even when its type name is changed.

struct EntityIdentifier

A type that uniquely identifies a specific instance of an app entity.

