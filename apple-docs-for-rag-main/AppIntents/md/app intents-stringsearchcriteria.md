

- App Intents
-  StringSearchCriteria 

Structure

# StringSearchCriteria

A structure that represents a string-based search request.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+macOS 14.2+tvOS 17.2+visionOS 1.0+watchOS 10.2+

``` source
struct StringSearchCriteria
```

## Topics

### Operators

static func == (StringSearchCriteria, StringSearchCriteria) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(term: String)

### Instance Properties

var hashValue: Int

The hash value.

var term: String

The full search term given by the user.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias SearchScopes

typealias Specification

typealias UnwrappedType

typealias ValueType

### Type Properties

static var defaultResolverSpecification: some ResolverSpecification

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- SearchCriteria
- Sendable

## See Also

### Defining the search criteria

var criteria: Self.Criteria

**Required**

protocol SearchCriteria

associatedtype Criteria : SearchCriteria

**Required**

