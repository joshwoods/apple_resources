

- MusicKit
- MusicCatalogSearchSuggestionsResponse
-  MusicCatalogSearchSuggestionsResponse.Suggestion 

Structure

# MusicCatalogSearchSuggestionsResponse.Suggestion

An item that represents a suggestion in the search suggestions response.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Suggestion
```

## Topics

### Operators

static func == (MusicCatalogSearchSuggestionsResponse.Suggestion, MusicCatalogSearchSuggestionsResponse.Suggestion) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

let displayTerm: String

A term to display to the user to select from.

var hashValue: Int

The hash value.

var id: String

The unique identifier for the suggestion.

let searchTerm: String

The term to use as a search input when using this suggestion.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomStringConvertible Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Identifiable
- Sendable

