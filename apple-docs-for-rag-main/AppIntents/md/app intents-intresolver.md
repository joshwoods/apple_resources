

- App Intents
-  IntResolver 

Structure

# IntResolver

A resolver that validates an integer is within the parameter’s inclusive range.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct IntResolver
```

## Topics

### Resolving the type

func resolve(from: Int, context: IntentParameterContext&lt;Int>) async throws -> Int?

Converts the specified value into the expected data type.

### Operators

static func == (IntResolver, IntResolver) -> Bool

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

RangeCheckingResolver Implementations

Resolver Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- RangeCheckingResolver
- Resolver
- Sendable

## See Also

### Integer resolution

struct IntFromDoubleResolver

A resolver that converts a double into an integer using the specified rounding rule and validates the result is within the parameter’s inclusive range.

struct IntFromStringResolver

A resolver that converts a string into an integer in the specified base and validates the result is within the parameter’s inclusive range.

