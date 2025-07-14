

- App Intents
-  ResolverSpecification 

Protocol

# ResolverSpecification

An internal type that a resolver uses to convert data values.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol ResolverSpecification : Hashable, Sendable, Sequence where Self.Element == any Resolver
```

## Overview

Don’t use a ResolverSpecification type directly in your code. The system uses this type internally to manage the resolution process.

## Topics

### Getting the value type

associatedtype Output : _IntentValue

**Required**

## Relationships

### Inherits From

- Equatable
- Hashable
- Sendable
- Sequence

### Conforming Types

- EmptyResolverSpecification
- ResolverSpecificationBuilder.Specification

  Conforms when `Property` conforms to `_IntentValue`.

## See Also

### Managing the resolution process

struct EmptyResolverSpecification

struct StringSearchCriteriaFromStringResolverSpecificification

An internal type that a resolver uses to convert data values.

enum ResolverSpecificationBuilder

A result builder that declaratively specifies a set of resolvers.

