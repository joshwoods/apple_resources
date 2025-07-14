

- App Intents
-  StringFromIntResolver 

Structure

# StringFromIntResolver

A resolver that converts one or more integers into one or more strings.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct StringFromIntResolver where Input : _IntentValue, Output : _IntentValue, Output.ValueType == String
```

## Topics

### Resolving the type

func resolve(from: Input, context: IntentParameterContext&lt;Output>) async throws -> Output?

Converts the specified value into the expected data type.

### Operators

static func == (StringFromIntResolver&lt;Input, Output>, StringFromIntResolver&lt;Input, Output>) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

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

struct AttributedStringFromStringResolver

A resolver that converts a string into an attributed string.

struct StringFromDoubleResolver

A resolver that converts a double into a string.

