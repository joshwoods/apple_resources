

- MusicKit
-  MusicLibrarySearchRequest 

Structure

# MusicLibrarySearchRequest

A request that your app uses to fetch items from user’s library using a search term.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 14.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct MusicLibrarySearchRequest
```

## Topics

### Operators

static func == (MusicLibrarySearchRequest, MusicLibrarySearchRequest) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(term: String, types: [any MusicLibrarySearchable.Type])

Creates a library search request for a specified search term and list of library searchable types.

### Instance Properties

var hashValue: Int

The hash value.

var includeTopResults: Bool

A Boolean value that indicates whether to request top search results.

var limit: Int

A limit for the number of items to return in the library search response.

let term: String

The search term for the request.

var types: [any MusicLibrarySearchable.Type]

The list of requested library searchable types.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

func response() async throws -> MusicLibrarySearchResponse

Fetches items of the requested library searchable types that match the search term of the request.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

