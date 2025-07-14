

- App Intents
-  Resolver 

Protocol

# Resolver

An interface to convert a value from one type to a different type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol Resolver : Hashable, Sendable
```

## Topics

### Resolving the type

func resolve(from: Self.Input, context: IntentParameterContext&lt;Self.Output>) async throws -> Self.Output?

Converts the specified value into the expected data type.

**Required**

associatedtype Input : _IntentValue

**Required**

associatedtype Output : _IntentValue

**Required**

### Managing the resolution process

protocol ResolverSpecification

An internal type that a resolver uses to convert data values.

struct EmptyResolverSpecification

struct StringSearchCriteriaFromStringResolverSpecificification

An internal type that a resolver uses to convert data values.

enum ResolverSpecificationBuilder

A result builder that declaratively specifies a set of resolvers.

### Type Aliases

typealias Context

## Relationships

### Inherits From

- Equatable
- Hashable
- Sendable

### Inherited By

- RangeCheckingResolver

### Conforming Types

- AttributedStringFromStringResolver
- BoolFromStringResolver
- DoubleFromIntResolver
- DoubleFromStringResolver
- DoubleResolver
- IntFromDoubleResolver
- IntFromStringResolver
- IntResolver
- StringFromDoubleResolver
- StringFromIntResolver
- StringSearchCriteriaFromStringResolverSpecificification
- URLFromStringResolver

