

- App Intents
-  IntFromDoubleResolver 

Structure

# IntFromDoubleResolver

A resolver that converts a double into an integer using the specified rounding rule and validates the result is within the parameter’s inclusive range.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct IntFromDoubleResolver
```

## Topics

### Creating the resolver

init(roundingRule: FloatingPointRoundingRule)

### Resolving the type

func resolve(from: Double, context: IntentParameterContext&lt;Int>) async throws -> Int?

Converts the specified value into the expected data type.

### Getting the rounding rule

var roundingRule: FloatingPointRoundingRule

### Operators

static func == (IntFromDoubleResolver, IntFromDoubleResolver) -> Bool

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

struct IntFromStringResolver

A resolver that converts a string into an integer in the specified base and validates the result is within the parameter’s inclusive range.

struct IntResolver

A resolver that validates an integer is within the parameter’s inclusive range.

