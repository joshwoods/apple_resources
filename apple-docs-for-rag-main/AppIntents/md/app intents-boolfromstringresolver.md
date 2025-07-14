

- App Intents
-  BoolFromStringResolver 

Structure

# BoolFromStringResolver

A resolver that converts a string into a Boolean, optionally using a localized display name.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct BoolFromStringResolver
```

## Topics

### Resolving the type

func resolve(from: String, context: IntentParameterContext&lt;Bool>) async throws -> Bool?

Converts the specified value into the expected data type.

### Operators

static func == (BoolFromStringResolver, BoolFromStringResolver) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias Input

typealias Output

### Default Implementations

Equatable Implementations

Resolver Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Resolver
- Sendable

