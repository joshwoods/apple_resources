

- App Intents
- ResolverSpecificationBuilder
-  ResolverSpecificationBuilder.Specification 

Structure

# ResolverSpecificationBuilder.Specification

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct Specification where Output : _IntentValue, repeat each R : Resolver
```

Available when `Property` conforms to `_IntentValue`.

## Topics

### Operators

static func == (ResolverSpecificationBuilder&lt;Property>.Specification&lt;Output, repeat each R>, ResolverSpecificationBuilder&lt;Property>.Specification&lt;Output, repeat each R>) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

func makeIterator() -> Array&lt;any Resolver>.Iterator

Returns an iterator over the elements of this sequence.

### Type Aliases

typealias Element

A type representing the sequence’s elements.

typealias Iterator

A type that provides the sequence’s iteration interface and encapsulates its iteration state.

### Default Implementations

Equatable Implementations

Sequence Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- ResolverSpecification
- Sendable
- Sequence

