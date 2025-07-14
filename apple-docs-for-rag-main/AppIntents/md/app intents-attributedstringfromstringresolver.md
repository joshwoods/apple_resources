

- App Intents
-  AttributedStringFromStringResolver 

Structure

# AttributedStringFromStringResolver

A resolver that converts a string into an attributed string.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct AttributedStringFromStringResolver
```

## Topics

### Resolving the type

func resolve(from: String, context: IntentParameterContext&lt;AttributedString>) async throws -> AttributedString?

Converts the specified value into the expected data type.

### Operators

static func == (AttributedStringFromStringResolver, AttributedStringFromStringResolver) -> Bool

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

## See Also

### String resolution

struct StringFromDoubleResolver

A resolver that converts a double into a string.

struct StringFromIntResolver

A resolver that converts one or more integers into one or more strings.

