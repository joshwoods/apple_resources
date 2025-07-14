

- App Intents
-  EmptyResolverSpecification 

Structure

# EmptyResolverSpecification

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct EmptyResolverSpecification where Value : _IntentValue
```

## Topics

### Creating the specification type

init()

### Iterating over the values

func makeIterator() -> IndexingIterator&lt;[any Resolver]>

Returns an iterator over the elements of this sequence.

typealias Output

### Operators

static func == (EmptyResolverSpecification&lt;Value>, EmptyResolverSpecification&lt;Value>) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

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

## See Also

### Managing the resolution process

protocol ResolverSpecification

An internal type that a resolver uses to convert data values.

struct StringSearchCriteriaFromStringResolverSpecificification

An internal type that a resolver uses to convert data values.

enum ResolverSpecificationBuilder

A result builder that declaratively specifies a set of resolvers.

