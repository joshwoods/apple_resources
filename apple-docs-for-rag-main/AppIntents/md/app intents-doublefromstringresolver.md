

- App Intents
-  DoubleFromStringResolver 

Structure

# DoubleFromStringResolver

A resolver that converts a string into a double and validates the result is within the parameter’s inclusive range.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct DoubleFromStringResolver
```

## Topics

### Resolving the type

func resolve(from: String, context: IntentParameterContext&lt;Double>) async throws -> Double?

Converts the specified value into the expected data type.

### Operators

static func == (DoubleFromStringResolver, DoubleFromStringResolver) -> Bool

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

### Floating-point resolution

struct DoubleFromIntResolver

struct DoubleResolver

A resolver that validates a double is within the parameter’s inclusive range.

