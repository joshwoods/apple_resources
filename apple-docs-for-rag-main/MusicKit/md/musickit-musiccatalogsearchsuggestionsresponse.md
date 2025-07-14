

- MusicKit
-  MusicCatalogSearchSuggestionsResponse 

Structure

# MusicCatalogSearchSuggestionsResponse

An object that contains results for a catalog search suggestions request.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct MusicCatalogSearchSuggestionsResponse
```

## Topics

### Structures

struct Suggestion

An item that represents a suggestion in the search suggestions response.

### Operators

static func == (MusicCatalogSearchSuggestionsResponse, MusicCatalogSearchSuggestionsResponse) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

let suggestions: [MusicCatalogSearchSuggestionsResponse.Suggestion]

A collection of suggested terms.

let topResults: MusicItemCollection&lt;MusicCatalogSearchSuggestionsResponse.TopResult>

A collection of top results.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias TopResult

A type alias for an item that represents one of the top results in a catalog search suggestions response.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomStringConvertible Implementations

Decodable Implementations

Encodable Implementations

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
- Sendable

