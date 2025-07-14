

- MusicKit
-  MusicCatalogSearchSuggestionsRequest 

Structure

# MusicCatalogSearchSuggestionsRequest

A request that your app uses to fetch suggestions from the Apple Music catalog using a search term.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct MusicCatalogSearchSuggestionsRequest
```

## Topics

### Initializers

init(term: String, includingTopResultsOfTypes: [any MusicCatalogSearchable.Type])

Creates a catalog search suggestions request for a specified search term along with a list of types to include when fetching top results.

### Instance Properties

var limit: Int?

A limit for the number of items to return in the catalog search suggestions response.

let term: String

The search term for the request.

var typesForTopResults: [any MusicCatalogSearchable.Type]

The list of requested types for top results.

### Instance Methods

func response() async throws -> MusicCatalogSearchSuggestionsResponse

Fetches suggestions of the requested catalog searchable types that match the search term of the request.

