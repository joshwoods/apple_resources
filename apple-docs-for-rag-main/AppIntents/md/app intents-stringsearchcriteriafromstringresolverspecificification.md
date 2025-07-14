

- App Intents
-  StringSearchCriteriaFromStringResolverSpecificification 

Structure

# StringSearchCriteriaFromStringResolverSpecificification

An internal type that a resolver uses to convert data values.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+macOS 14.2+tvOS 17.2+visionOS 1.0+watchOS 10.2+

``` source
struct StringSearchCriteriaFromStringResolverSpecificification
```

## Overview

Don’t use a `StringSearchCriteriaFromStringResolverSpecificification` type directly in your code. The system uses this type internally to manage the resolution process.

## Topics

### Resolving the type

func resolve(from: String, context: IntentParameterContext&lt;StringSearchCriteria>) async throws -> StringSearchCriteria?

Converts the specified value into the expected data type.

### Operators

static func == (StringSearchCriteriaFromStringResolverSpecificification, StringSearchCriteriaFromStringResolverSpecificification) -> Bool

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

### Managing the resolution process

protocol ResolverSpecification

An internal type that a resolver uses to convert data values.

struct EmptyResolverSpecification

enum ResolverSpecificationBuilder

A result builder that declaratively specifies a set of resolvers.

